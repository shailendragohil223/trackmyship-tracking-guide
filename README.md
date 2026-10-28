# Track My Ship – Courier and Parcel Tracking Guide for India

[Track My Ship](https://trackmyship.co/) is a free, independent website for checking the status of parcels sent with courier companies in India. Enter the courier's tracking number (AWB or consignment number) and the site shows the latest status, the scan history and the parcel's route on a map, for several couriers in one place.

This repository is a plain-language reference for **shipment tracking**: which couriers the site covers, which tracking numbers work, what common tracking terms and statuses mean, and what to do when tracking shows nothing. It documents the website and general courier tracking concepts. It does not contain the website's source code and does not provide an API.

- **Website:** https://trackmyship.co/
- **Full parcel tracking guide:** https://trackmyship.co/parcel-tracking-guide

> [!NOTE]
> Track My Ship shows the tracking information that couriers publish. For official confirmation, delivery problems, claims or details not shown in tracking, use the courier's own website or customer support.

## Contents

- [Features](#features)
- [Which tracking numbers work](#which-tracking-numbers-work)
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

- **Courier tracking by AWB or consignment number** for the couriers listed [below](#supported-courier-services).
- **Automatic courier detection** for common DTDC, Blue Dart, Delhivery and Speed Post number formats. For other couriers, choose the courier from the list next to the search box, or use that courier's tracking page.
- **Tracking details in one view:** the current status, a tracking history with each scan's date, time and place, and the parcel's route on a map (map data © OpenStreetMap contributors).
- **Expected delivery date** when the courier provides one. This is the courier's estimate, not a guarantee.
- **Shareable tracking links** in the form `https://trackmyship.co/?q=<tracking-number>`, which open straight to the result.
- **Courier-specific tracking pages** with the courier already selected, plus notes on where to find that courier's number and whom to contact about a problem.
- **A parcel tracking guide** explaining tracking numbers, status meanings, delays and failed deliveries.
- **No account needed:** tracking is free and needs no sign-up or login.

## Which tracking numbers work

Track My Ship tracks **courier tracking numbers only**. Other identifiers are rejected with a message explaining where to track them instead.

| You have | Works on Track My Ship? | Where to track it instead |
|---|---|---|
| AWB number | Yes | – |
| Consignment or docket number | Yes | – |
| Waybill number (e.g. Delhivery) | Yes | – |
| Speed Post article number (e.g. `EE123456789IN`) | Yes | – |
| Mobile number | No | Ask the sender or seller for the courier tracking number |
| Email address | No | Check the seller's shipping email for the tracking number |
| LR (lorry receipt) number | No | The road transporter's own website |
| Shop order ID | No | The seller's website or app, which usually shows the courier and tracking number |

## Supported courier services

| Courier | Tracking page | Detected automatically from the number |
|---|---|---|
| DTDC | [trackmyship.co/dtdc-tracking](https://trackmyship.co/dtdc-tracking) | Yes |
| Blue Dart | [trackmyship.co/bluedart-tracking](https://trackmyship.co/bluedart-tracking) | Yes |
| Delhivery | [trackmyship.co/delhivery-tracking](https://trackmyship.co/delhivery-tracking) | Yes |
| Speed Post (India Post) | [trackmyship.co/speed-post-tracking](https://trackmyship.co/speed-post-tracking) | Yes |
| Trackon Couriers | [trackmyship.co/trackon-tracking](https://trackmyship.co/trackon-tracking) | No – select the courier |
| The Professional Couriers | [trackmyship.co/professional-courier-tracking](https://trackmyship.co/professional-courier-tracking) | No – select the courier |
| ST Courier | [trackmyship.co/st-courier-tracking](https://trackmyship.co/st-courier-tracking) | No – select the courier |
| Shree Maruti Courier | [trackmyship.co/shree-maruti-courier-tracking](https://trackmyship.co/shree-maruti-courier-tracking) | No – select the courier |
| Shree Anjani Courier | [trackmyship.co/shree-anjani-courier-tracking](https://trackmyship.co/shree-anjani-courier-tracking) | No – select the courier |
| Shree Tirupati Courier | [trackmyship.co/shree-tirupati-courier-tracking](https://trackmyship.co/shree-tirupati-courier-tracking) | No – select the courier |

The courier list on the website comes from its tracking data provider, so it may include more couriers than this table and may change over time. Track My Ship is not affiliated with any of these couriers.

## How to track a shipment

1. Find your tracking number on the booking receipt, or in the seller's shipping SMS, email or order page.
2. Go to [trackmyship.co](https://trackmyship.co/), or to your courier's tracking page from the [table above](#supported-courier-services).
3. Type the number into the tracking box, without spaces.
4. Leave the courier on **Detect courier**, or choose your courier from the list. On a courier's own tracking page, the courier is already selected.
5. Press **Track**.
6. Review the result: the current status, the tracking history and the route on the map.

Results depend on what the courier has published. A newly booked shipment may show nothing for a few hours, sometimes until the next working day, because the courier hasn't recorded its first scan yet.

## Useful tracking resources

| Page | What it covers |
|---|---|
| [Track My Ship homepage](https://trackmyship.co/) | The main tracker |
| [Parcel tracking guide](https://trackmyship.co/parcel-tracking-guide) | Tracking numbers, statuses, delays and failed deliveries |
| [Types of tracking number](https://trackmyship.co/parcel-tracking-guide#tracking-numbers) | AWB, consignment, waybill, Speed Post and LR numbers |
| [Tracking status meanings](https://trackmyship.co/parcel-tracking-guide#statuses) | What each status means and what to do |
| [Delayed or failed delivery](https://trackmyship.co/parcel-tracking-guide#delayed) | Steps to take when a parcel is stuck or returned |
| [About and contact](https://trackmyship.co/contact) | Who runs the site and how to reach them |
| [Terms of Use](https://trackmyship.co/terms) | Fair-use rules and limits of the service |

## Tracking terminology

Couriers use different names for the same things, and exact status wording varies from courier to courier. These are general meanings.

### Tracking numbers

| Term | Meaning |
|---|---|
| **Tracking number** | The general name for the reference a courier assigns to a shipment when it is booked. Every scan of the parcel is recorded against it. |
| **AWB number** | Short for "air waybill" number. Many Indian express couriers use this term for all their shipments, including those sent by road. |
| **Consignment number** | The courier's reference for your shipment, usually printed on the booking receipt. Some couriers call it a docket number. |

An **order ID** from a shopping site is not a tracking number, and neither is an **LR number** from a road transporter. See [Which tracking numbers work](#which-tracking-numbers-work).

### Common statuses

| Status | Meaning |
|---|---|
| **Shipment booked** | The shipment has been created in the courier's system but hasn't been collected or handed over yet. |
| **In transit** | The parcel is moving through the courier's network of hubs and branches toward the destination. Gaps between scans are normal. |
| **Out for delivery** | The parcel is with a delivery person and is expected to arrive that day. |
| **Delivered** | The courier has recorded the parcel as handed over at the delivery address. |
| **Tracking information unavailable** | No scans can be shown for the number yet. Common reasons are a very recent booking, a typing mistake or the wrong courier being selected. |

The website's guide also explains *Picked up*, *Delayed / Exception* and *Returning to origin (RTO)*: see [tracking status meanings](https://trackmyship.co/parcel-tracking-guide#statuses).

## Troubleshooting

| Problem | What to try |
|---|---|
| **Invalid tracking number** | Re-check each character. Watch for the letter O versus zero, the letter I versus one, and missing digits. |
| **Mobile number, email, LR number or order ID rejected** | These aren't supported. Get the courier tracking number from the sender, the seller's shipping message or the order page. See [Which tracking numbers work](#which-tracking-numbers-work). |
| **Courier not detected** | Automatic detection only covers DTDC, Blue Dart, Delhivery and Speed Post formats. Choose your courier from the list, or use the courier's tracking page. |
| **Wrong courier selected** | Choose the courier named on your receipt or shipping message. Different couriers' numbers can look alike. |
| **Tracking number not found** | Confirm the number and courier with the sender or seller. If it still isn't found after a day, check the courier's own website. |
| **Tracking number generated recently** | Wait a few hours and try again. The first scan often appears only after the courier collects the parcel. |
| **Status not updated** | Couriers add scans only when a parcel is handled at a hub or branch, so long journeys can show no change for a day or more. If nothing changes for about 48 hours, contact the courier or the sender. |
| **Courier website shows different information** | The courier's own website is the official source. Recent results may be briefly cached, and updates can take time to reach third-party trackers, so rely on the courier's website and contact the courier if anything needs action. |

For delays, damage, address changes or failed deliveries, contact the courier or the sender directly. They hold the parcel and can act on it; a tracking website cannot.

## Developer information

> [!IMPORTANT]
> **Track My Ship does not offer a public API.** There are no public endpoints, API keys, SDKs or integration packages, and this repository contains no code.

You can use this repository as:

- A reference for the tracking terminology used by Indian couriers: AWB, consignment, docket, waybill and Speed Post article numbers, and common status meanings.
- A list of the couriers the site covers, with links to each courier's tracking page.
- A starting point for user-facing help text in your own shipping or e-commerce project. Please write it in your own words; see [License](#license).

If you need programmatic tracking, use the courier's official channels or a tracking data provider directly. Don't scrape trackmyship.co or send automated searches to it: the [Terms of Use](https://trackmyship.co/terms) forbid bulk or automated searching, and searches are rate-limited.

For linking to a specific result from your own app or message, the shareable link format `https://trackmyship.co/?q=<tracking-number>` is described in the website's [privacy policy](https://trackmyship.co/privacy-policy). It is a web page link, not an API.

## Privacy and security

This repository is public. When opening an issue or pull request, please **do not post**:

- Tracking numbers for real or private shipments
- Names, addresses, phone numbers or email addresses
- Screenshots of booking receipts, labels or tracking results that show personal details
- Passwords, API keys or other credentials

Use clearly made-up example numbers when you need to illustrate a format. For questions about a specific shipment, contact the courier. For questions about the website, email info@trackmyship.co.

Anyone who has a tracking number or a shareable tracking link can see that shipment's status, so share them only with people who need them. Under the website's [Terms of Use](https://trackmyship.co/terms), only track shipments you sent, are receiving or are authorised to track.

Read how the website handles the tracking numbers you enter in the [Track My Ship privacy policy](https://trackmyship.co/privacy-policy).

## Disclaimer

Track My Ship is an independent, third-party tracking website. It is not a courier company and is not affiliated with, endorsed by or sponsored by any of the couriers mentioned here. Courier names and trademarks belong to their respective owners and are used only to identify the services being tracked.

Tracking availability and accuracy depend on the courier and the data it publishes, and delivery dates are estimates. For official confirmation, use the courier's own website. See also the website's [Terms of Use](https://trackmyship.co/terms).

## Contributing

Documentation improvements are welcome, such as clearer explanations, corrected status meanings or fixed links.

1. Fork this repository.
2. Create a branch for your change.
3. Make a focused documentation change.
4. Open a pull request describing what you changed and why.

See [CONTRIBUTING.md](CONTRIBUTING.md) for details. Please follow the [privacy guidance](#privacy-and-security) in all issues and pull requests.

## License

Licensing terms for this repository have not been specified yet. Until a license is added, please ask before reusing this documentation elsewhere.
