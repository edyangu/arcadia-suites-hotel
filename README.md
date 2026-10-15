Arcadia Suites Hotel Kampala

Official website for Arcadia Suites Hotel, a boutique hotel on Kira Road, Kampala, Uganda.

Live site: https://arcadia-suites-hotel.vercel.app


WHAT THIS IS

A modern hotel website with a full admin dashboard. All content is managed from the admin panel and updates on the public site within seconds.

Guests can view rooms, browse the rooftop restaurant menu, see hotel amenities and location, and submit booking enquiries that arrive by email and appear in the admin dashboard.


PAGES

index.html       Homepage
rooms.html       All room types
room.html        Single room detail
dining.html      Rooftop restaurant and menu
amenities.html   Hotel facilities
location.html    Map and nearby landmarks
about.html       Hotel story and values
contact.html     Contact details and map
booking.html     Booking enquiry form
privacy.html     Privacy policy
terms.html       Terms of service
404.html         Custom error page
admin.html       Admin dashboard (login required)


HOW IT WORKS

Public site
Reads live data from Firebase Firestore. When admin updates anything, the public site reflects it within seconds.

Booking form
Submits to Formspree (sends email) and Firestore (stores enquiry for admin panel).

Admin panel
Password protected via Firebase Authentication. Only the admin email can log in.

Images
Uploaded to postimages.org (free), then the direct link is pasted into the admin panel. No image files are stored in this repo.


ADMIN PANEL

Access at /admin.html

Enquiries       Booking requests from the website
Rooms           Room types, prices, photos, amenities
Menu            Restaurant dishes by category
Photos          Gallery images
Offers          Promotional popups shown on the public site
Reviews         Guest testimonials
Settings        Hotel name, phone, email, address, WhatsApp

Every change made in admin appears on the public site immediately.


TECH STACK

Static HTML, CSS, and JavaScript
Firebase Firestore (database)
Firebase Authentication (admin login)
Formspree (email delivery for booking enquiries)
Vercel (hosting)
Google Fonts (typography)

No build step. No framework. No npm. The site is served as-is.


FIRESTORE COLLECTIONS

rooms        Room types with prices, photos, amenities
menu         Restaurant items by category
photos       Gallery images
offers       Promotional popups
reviews      Guest testimonials
enquiries    Booking form submissions
settings     Hotel information (single document)


SECURITY

Firestore rules are set so:

Anyone can read rooms, menu, photos, offers, reviews, and settings
Anyone can create a booking enquiry
Only logged-in admin can write any content or read enquiries

Admin authentication is handled by Firebase. No password is stored in the code.


DEPLOYING CHANGES

The repo is connected to Vercel. Any commit to the main branch triggers a new deployment automatically, live within 30 seconds.

Manual deploy: import the repo at vercel.com/new and click Deploy.


CONTACT

Arcadia Suites Hotel
Kira Road, Kampala, Uganda
Phone: +256 200 950 700
Email: info@arcadiasuiteshotel.com
WhatsApp: https://wa.me/256200950700
Website: https://arcadiasuiteshotel.com


BUILT BY

Samuel Edyangu
October 2026


LICENSE

Copyright 2026 Arcadia Suites Hotel. All rights reserved.
