# Amavante Technologies Company Limited

A responsive, single-page business website for Amavante Technologies Company Limited, based in Kireka, Kampala, Uganda. The site introduces the company, its digital technology services, ICT training academy, internship opportunities, contact channels, and current MTN Mobile Money payment instructions.

## Website sections

- **Services:** technology, software, design, consulting, security, and digital services.
- **About:** company mission, vision, and core values.
- **ICT Training Academy:** courses available by enquiry.
- **Internships:** departments accepting applications.
- **Payments:** MTN merchant payment instructions and a form for submitting a transaction reference for manual verification.
- **Contact:** email, telephone, WhatsApp, and a contact form.

## Project files

- `index.html` — complete website, including its styles, content, and client-side JavaScript.

The site has no build step, package manager, or server-side application.

## Run locally

Open `index.html` in a browser. To run it through the included XAMPP Apache server, place the project in the web root and visit:

```text
http://localhost/Amavante-Technologies/
```

## Current payment workflow

The payment section provides MTN merchant codes and asks the customer to make a payment through MTN MoMo, then submit the transaction reference. The page saves submissions in that browser's `localStorage` as pending and opens the customer's email app with a verification message addressed to the company.

This is a **manual reference-submission workflow**, not a payment gateway integration. The website does not initiate a mobile-money charge, receive a payment callback, or verify that funds arrived. Browser-local submissions are not shared with the business or other devices, and opening an email draft does not send it automatically. Staff must verify each payment independently before treating it as paid.

Before accepting payments through an automated mobile-money integration, connect the site to a trusted payment provider or merchant API through a backend. Keep API credentials and payment verification on the server, validate provider callbacks, and never collect or request a customer's MoMo PIN on the website.

## Updating the site

Edit `index.html`. The service list, values, courses, internship departments, merchant details, and contact email are defined in the JavaScript near the end of the file. The page currently uses no external libraries.
