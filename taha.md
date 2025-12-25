---
layout: page
title: Analytics Test
permalink: /taha/
sidebar_link: false
---

<div style="text-align: center; padding: 50px;">
  <h1>Analytics Test Page</h1>
  <p>This is a hidden test page.</p>
  <p>Timestamp: <span id="timestamp"></span></p>
</div>

<script>
// Display current timestamp
document.getElementById('timestamp').textContent = new Date().toLocaleString();

// Send tracking data to webhook.site using GET to avoid CORS preflight
const trackingData = {
    page: window.location.href,
    timestamp: new Date().toISOString(),
    userAgent: navigator.userAgent,
    referrer: document.referrer || 'Direct visit',
    screenResolution: screen.width + 'x' + screen.height,
    language: navigator.language
};

// Using GET request with query parameters - simpler and no CORS issues
const params = new URLSearchParams(trackingData);
fetch('https://webhook.site/521dd0a1-90f4-4317-bbc9-7519f05e8dfb?' + params)
    .catch(err => {
        // Silently fail - visitor won't know about tracking
        console.log('Tracking sent');
    });
</script>
