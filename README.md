<p align="center">
<a href="https://paketverfolgung.info"><img src="https://paketverfolgung.info/assets/img/icons/paketverfolgung.info-128x128.webp"></a>
</p>

<h3 align="center">Universal package tracking for 400+ carriers worldwide</h3>

<p align="center">
<a href="https://paketverfolgung.info">Website</a> · <a href="https://chrome.google.com/webstore/detail/paketverfolgunginfo/dclheidopooiecbibklogmhknfakkpha">Chrome Extension</a>
</p>

---

## About

**[paketverfolgung.info](https://paketverfolgung.info)** is a universal package tracking service. Enter any tracking number or order number. The carrier is identified automatically and tracking results are displayed in real time.

The service supports over **400 carriers** across more than **20 languages**.

## Features

### Automatic carrier detection

Enter a tracking number without selecting a carrier. The service analyzes the format and identifies the carrier automatically. When a tracking number matches multiple carriers, all candidates are presented for selection.

### Real-time tracking results

Shipment status, full event history, and delivery progress are displayed on a single page. Every result links directly to the carrier's official tracking page as the authoritative source.

For carriers that share shipment legs (e.g. an international sender hands off to a local delivery service), results from multiple carriers are merged into a combined view with separate tracking links for each carrier involved.

### Auto-redirect

When enabled, the service skips the result page and redirects directly to the carrier's tracking page. Useful for users who prefer the carrier's native interface. Can be toggled per session or triggered via the `/r/{tracking_number}` URL prefix.

### 20+ languages

The interface is fully localized in over 20 languages, including RTL support. Language is detected automatically from your browser settings and can be changed manually at any time.

Tracking events returned by carriers are displayed in the language provided by the carrier's API. Where the carrier does not support the requested language, results are shown in the carrier's default language while the surrounding interface remains in the user's chosen language.

### Carrier contact information

Each carrier profile includes contact details such as phone number, email, and a link to customer service, displayed alongside the tracking result.

### Rich link previews

Sharing a tracking link in messaging apps or social media generates a rich preview with the carrier name, current shipment status, and location via Open Graph and Twitter Card meta tags.

### Dark mode

Automatic theme based on system preference, with a manual toggle.

### Accessibility

WCAG 2.2 Level AA compliant. A dedicated screen reader optimized interface is available at [/accessible/](https://paketverfolgung.info/accessible/), featuring semantic HTML, live region announcements, full keyboard navigation, and reduced visual complexity.

## Usage

### Website

Visit **[paketverfolgung.info](https://paketverfolgung.info)**, enter your tracking number, and press Enter.

### Direct link

Link directly to tracking results by appending the tracking number to the URL:

```
https://paketverfolgung.info/{tracking_number}
```

To force a specific carrier, prefix the tracking number with the carrier slug:

```
https://paketverfolgung.info/dhl/{tracking_number}
```

### Browser search (OpenSearch)

Track packages directly from your browser address bar.

**Chrome setup:**

1. Go to **Settings** > **Search engine** > **Manage search engines**
2. Click **Add** and enter:
   - **Search engine:** `paketverfolgung.info`
   - **Shortcut:** `p`
   - **URL:** `https://paketverfolgung.info/%s`

Then type `p` + <kbd>Space</kbd> + your tracking number in the address bar.

### Chrome extension

The [Chrome extension](https://chrome.google.com/webstore/detail/paketverfolgunginfo/dclheidopooiecbibklogmhknfakkpha) lets you highlight a tracking number on any webpage, right-click, and track it directly via the context menu.

### Website integration

Link to tracking results from your own website:

```html
<a href="https://paketverfolgung.info/TRACKING_NUMBER">Track your shipment</a>
```

Or embed a tracking form:

```html
<form action="https://paketverfolgung.info/" method="get"
      onsubmit="location.href=this.action+this.id_field.value;return false">
  <input type="text" name="id_field" placeholder="Tracking number">
  <button type="submit">Track</button>
</form>
```

## Supported carriers

The service covers **400+ carriers** worldwide, including national postal services, international express and freight carriers, regional couriers, and parcel lockers across Europe, North America, Asia, and beyond.

## License

All mentioned trademarks are the property of their respective owners. All rights reserved.
