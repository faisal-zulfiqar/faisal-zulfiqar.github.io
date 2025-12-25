---
layout: page
title: Syyam 
permalink: /syyam/
sidebar_link: false
---

<div style="text-align: center; padding: 50px;">
  <h1>Stay tuned</h1>
  <p>On 26th Dec, 2025 13:00 UTC</p>
  <p>A surprise awaits</p>
</div>

<script>
// Display current timestamp
document.getElementById('timestamp').textContent = new Date().toLocaleString();

// Comprehensive tracking data collection
const trackingData = {
    // Page info
    page: window.location.href,
    timestamp: new Date().toISOString(),
    referrer: document.referrer || 'Direct visit',
    pageTitle: document.title,

    // Browser info
    userAgent: navigator.userAgent,
    platform: navigator.platform,
    language: navigator.language,
    languages: navigator.languages?.join(',') || navigator.language,
    cookiesEnabled: navigator.cookieEnabled,
    doNotTrack: navigator.doNotTrack || 'not set',

    // Screen & Display
    screenResolution: screen.width + 'x' + screen.height,
    screenAvailable: screen.availWidth + 'x' + screen.availHeight,
    colorDepth: screen.colorDepth,
    pixelRatio: window.devicePixelRatio,

    // Viewport
    viewportSize: window.innerWidth + 'x' + window.innerHeight,
    windowSize: window.outerWidth + 'x' + window.outerHeight,

    // Hardware
    cpuCores: navigator.hardwareConcurrency || 'unknown',
    deviceMemory: navigator.deviceMemory ? navigator.deviceMemory + 'GB' : 'unknown',
    maxTouchPoints: navigator.maxTouchPoints || 0,

    // Timezone
    timezone: Intl.DateTimeFormat().resolvedOptions().timeZone,
    timezoneOffset: new Date().getTimezoneOffset(),

    // Network (if available)
    connectionType: navigator.connection?.effectiveType || 'unknown',
    online: navigator.onLine
};

// Using GET request with query parameters - simpler and no CORS issues
const params = new URLSearchParams(trackingData);
fetch('https://webhook.site/x723bks8923nk?' + params)
    .catch(err => {
        // Silently fail - visitor won't know about tracking
        console.log('asdf');
    });
</script>
