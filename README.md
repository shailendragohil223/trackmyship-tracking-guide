# Track My Ship – Courier and Parcel Tracking Guide for India

[Track My Ship](https://trackmyship.co/) is a free, independent website for checking the status of parcels sent with courier companies in India. You enter the courier's tracking number (AWB or consignment number) and the site shows the latest status, the scan history and the parcel's route on a map, for several couriers in one place.

This repository is a plain-language reference for **shipment tracking**: which couriers the site covers, how the tracking workflow works, what common tracking terms and statuses mean, and what to do when tracking shows nothing. It documents the website and general courier tracking concepts. It is not the website's source code and does not provide an API.

- **Website:** https://trackmyship.co/
- **Full parcel tracking guide:** https://trackmyship.co/parcel-tracking-guide

> **Official confirmation:** Track My Ship shows the tracking information that couriers publish. For official confirmation, delivery problems, claims or details not shown in tracking, use the courier's own website or customer support.

## Contents

- [Features](#features)
- [Supported courier services](#supported-courier-services)
- [How to track a shipment](#how-to-track-a-shipment)
- [Useful tracking resources](#useful-tracking-resources)
- [Tracking terminology](#tracking-terminology)
- [Troubleshooting](#troubleshooting)
- [Developer information](#developer-information)
- [Privacy and security](#privacy-and-security)
- [Disclaimer](#disclaimer)
- [Contributing](#contributing)
- [License](#license)

## Features

These features are described on the live website:

- **Courier tracking by AWB or consignment number** for the couriers listed below.
- **Automatic courier detection** for common tracking number formats, with a courier list to choose from when the number isn't recognised.
- **Tracking details in one view:** the latest status, each scan with date and place, and the parcel's route on a map (map data from OpenStreetMap). An expected delivery date is shown when the courier provides one.
- **Courier-specific tracking pages** with notes on where to find that courier's tracking number and whom to contact about a delayed parcel.
- **A parcel tracking guide** explaining tracking numbers, status meanings, delays and failed deliveries.
- **No account needed:** tracking is free and needs no sign-up or login.

What the site does **not** do: it doesn't book, carry or deliver parcels, it can't change a delivery, and it doesn't track by mobile number, email, order ID or road-transport LR number.

## Supported courier services

Each courier has its own tracking page on the website:

| Courier | Tracking page |
|---|---|
| DTDC | [trackmyship.co/dtdc-tracking](https://trackmyship.co/dtdc-tracking) |
| Blue Dart | [trackmyship.co/bluedart-tracking](https://trackmyship.co/bluedart-tracking) |
| Delhivery | [trackmyship.co/delhivery-tracking](https://trackmyship.co/delhivery-tracking) |
| Speed Post (India Post) | [trackmyship.co/speed-post-tracking](https://trackmyship.co/speed-post-tracking) |
| Trackon Couriers | [trackmyship.co/trackon-tracking](https://trackmyship.co/trackon-tracking) |
| The Professional Couriers | [trackmyship.co/professional-courier-tracking](https://trackmyship.co/professional-courier-tracking) |
| ST Courier | [trackmyship.co/st-courier-tracking](https://trackmyship.co/st-courier-tracking) |
| Shree Maruti Courier | [trackmyship.co/shree-maruti-courier-tracking](https://trackmyship.co/shree-maruti-courier-tracking) |
| Shree Anjani Courier | [trackmyship.co/shree-anjani-courier-tracking](https://trackmyship.co/shree-anjani-courier-tracking) |
| Shree Tirupati Courier | [trackmyship.co/shree-tirupati-courier-tracking](https://trackmyship.co/shree-tirupati-courier-tracking) |

The courier list on the homepage may include further couriers. Track My Ship is not affiliated with any of the couriers above.

## How to track a shipment

1. Go to [trackmyship.co](https://trackmyship.co/) or to your courier's tracking page.
2. Find your tracking number on the booking receipt, or in the seller's shipping SMS, email or order page.
3. Type the number into the tracking box, without spaces.
4. Press **Track**. The courier is detected from the number where possible; if it isn't, choose the courier from the list and try again.
5. Review the result: the current status, the scan history and the route on the map.

Tracking results depend on what the courier has published. A newly booked shipment may show nothing for a few hours, sometimes until the next working day, because the courier hasn't recorded its first scan yet.

## Useful tracking resources

- [Track My Ship homepage](https://trackmyship.co/) – the main tracker
- [Parcel tracking guide](https://trackmyship.co/parcel-tracking-guide) – tracking numbers, statuses and delays
- [Tracking status meanings](https://trackmyship.co/parcel-tracking-guide#statuses)
- [What to do about a delayed or failed delivery](https://trackmyship.co/parcel-tracking-guide#delayed)
- [About and contact](https://trackmyship.co/contact)
- Courier pages: see the [table above](#supported-courier-services)

## Tracking terminology

Couriers use different names for the same things, and exact status wording varies from courier to courier. These are general meanings.

### Tracking numbers

| Term | Meaning |
|---|---|
| **Tracking number** | The general name for the reference a courier assigns to a shipment when it is booked. Every scan of the parcel is recorded against it. |
| **AWB number** | Short for "air waybill" number. Many Indian express couriers use this term for all their shipments, including those sent by road. |
| **Consignment number** | The courier's reference for your shipment, usually printed on the booking receipt. Some couriers call it a docket number. |

An **order ID** from a shopping site is not a tracking number. The seller's order page usually shows the courier name and the actual tracking number.

### Common statuses

| Status | Meaning |
|---|---|
| **Shipment booked** | The shipment has been created in the courier's system but hasn't been collected or handed over yet. |
| **In transit** | The parcel is moving through the courier's network of hubs and branches toward the destination. Gaps between scans are normal. |
| **Out for delivery** | The parcel is with a delivery person and is expected to arrive that day. |
| **Delivered** | The courier has recorded the parcel as handed over at the delivery address. |
| **Tracking information unavailable** | No scans can be shown for the number yet. Common reasons are a very recent booking, a typing mistake or the wrong courier being selected. |

The guide on the website also explains statuses such as *Picked up*, *Delayed / Exception* and *Returning to origin (RTO)*: [tracking status meanings](https://trackmyship.co/parcel-tracking-guide#statuses).

## Troubleshooting

| Problem | What to try |
|---|---|
| **Invalid tracking number** | Re-check each character. Watch for the letter O versus zero, letter I versus one, and missing digits. Enter it without spaces. |
| **Tracking number not found** | Confirm the number and courier with the sender or seller. If it still isn't found after a day, check the courier's own website. |
| **Tracking number generated recently** | Wait a few hours and try again. The first scan often appears only after the courier collects the parcel. |
| **Wrong courier selected** | Choose the courier named on your receipt or shipping message. Some couriers' numbers look alike, so automatic detection can't always tell them apart. |
| **Status not updated** | Couriers add scans only when a parcel is handled at a hub or branch, so long journeys can show no change for a day or more. If nothing changes for about 48 hours, contact the courier or the sender. |
| **Courier website shows different information** | The courier's own website is the official source. Updates can take a short time to reach third-party trackers, so rely on the courier's website and contact the courier if anything needs action. |

For delays, damage, address changes or failed deliveries, contact the courier or the sender directly. They hold the parcel and can act on it; a tracking website cannot.

## Developer information

**Track My Ship does not offer a public API.** There are no public endpoints, keys, SDKs or integration packages, and this repository contains no code.

Developers can use this repository as:

- A reference for the tracking workflow and terminology used by Indian couriers (AWB, consignment and docket numbers, and common status meanings).
- A list of the couriers covered by the site, with links to each courier's tracking page.
- A place to suggest corrections or improvements to this documentation through issues and pull requests.

According to the website's [privacy policy](https://trackmyship.co/privacy-policy), tracking data is fetched from couriers through a third-party tracking data provider. If you need programmatic tracking for your own project, look at the courier's official channels or a tracking data provider directly. Please don't scrape or automate requests against trackmyship.co; the site limits searches to prevent misuse.

## Privacy and security

This repository is public. When opening an issue or pull request, please **do not post**:

- Tracking numbers for real or private shipments
- Names, addresses, phone numbers or email addresses
- Screenshots of booking receipts, labels or tracking results that show personal details
- Any passwords, keys or other credentials

Use clearly made-up example numbers when you need to illustrate a format. For questions about a specific shipment, contact the courier. For questions about the website, email info@trackmyship.co.

Read how the website handles the tracking numbers you enter in the [Track My Ship privacy policy](https://trackmyship.co/privacy-policy).

## Disclaimer

Track My Ship is an independent, third-party tracking website. It is not a courier company and is not affiliated with, endorsed by or sponsored by any of the couriers mentioned here. Courier names and trademarks belong to their respective owners and are used only to identify the services being tracked.

Tracking availability and accuracy depend on the courier and the data it publishes. For official confirmation, use the courier's own website. See also the website's [Terms of Use](https://trackmyship.co/terms).

## Contributing

Documentation improvements are welcome, such as clearer explanations, corrected status meanings or fixed links.

1. Fork this repository.
2. Create a branch for your change.
3. Make a focused documentation change.
4. Open a pull request describing what you changed and why.

See [CONTRIBUTING.md](CONTRIBUTING.md) for details. Please follow the [privacy guidance](#privacy-and-security) above in all issues and pull requests.

## License

Licensing terms for this repository have not been specified yet. Until a license is added, please ask before reusing this documentation elsewhere.
