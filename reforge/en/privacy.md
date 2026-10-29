---
title: Reforge privacy policy
permalink: /reforge/en/privacy/
lang: en
---

# Reforge privacy policy

*Last updated: 29 October 2026.* · [Version française](../../privacy/)

Reforge is an Android strength training coach. This page says what it stores, what can leave your phone, where it goes, and how you stay in control.

## In short

- **No account, no Reforge server.** The developer receives, stores and sells none of your data, apart from the order information Google Play gives any seller when you subscribe.
- **The subscription goes through Google Play**: payment, renewal and cancellation happen at Google, and Reforge never sees how you pay. See "Subscription".
- **No ads, no analytics, no tracking** by Reforge.
- **Everything stays on your phone**: your profile, your sessions, your weight, your meals, your conversation with the coach and your settings.
- **Four things can leave it**: the exercise illustrations it downloads; what you send to the coach's AI when it goes through the cloud, that is if you turned it on on a phone that can't run Gemini Nano (messages, meals to estimate, meal photos, and a summary of your profile, health and training); the barcode of a product you look up in Open Food Facts; and what you choose to exchange with Health Connect. Each is detailed below, and none is active without you.
- **Technical information** that Google's libraries built into the app may send to Google to work: see "Technical information sent to Google". Reforge receives none of it.

## What Reforge stores on your phone

- Your profile: goal, level, age, height, weight, equipment, training places, sensitive areas and the notes you write.
- Your program, your own exercises, your sessions and every set you do (load, reps, effort).
- Your weigh-ins and body fat, entered by you or imported from Health Connect.
- Your body measurements (waist, hips, arms…), if you enter any: they stay on your phone and in your backups, and are not sent to the AI.
- Your progress photos, if you take or choose any: they stay in the app's private storage and go nowhere else, not to the AI, not into the export, not into the automatic backup, not into Android's cloud backup. Only a direct transfer to a new phone (Android 12 and later, by cable or Wi-Fi) copies them. "Save a copy" writes the photo where you choose in Android's picker, and "Save my photos", on the subscription screen, copies them all to the folder you choose; a photo deleted in Reforge is erased from the phone.
- Your meals (time, description, foods and their estimated nutrients), your favorite meals and your nutrition settings, including your diet, your allergies and the foods you avoid if you entered them: this is health data, which you choose to enter (or not), and which stays on your phone and in your backups. Meal photos are not kept: one taken with Reforge's camera (or with the phone's camera app, if Reforge's can't open) is written to the app's cache, then erased as soon as Reforge has read it.
- The conversation with the coach, which you can erase with "New conversation".
- Your settings (theme, units, rest timer, training reminders, AI on or off, each widget's opacity and colors) and your rest habits.

This data is in the app's private storage: other apps can't reach it.

### Home screen widgets

If you add a Reforge widget to your home screen, it shows part of this data there: your weight and body fat over the last month ("Weight and body fat"), today's intake against your targets ("Today's intake"), or this week's sessions and today's ("My week"). The widget is drawn by your phone and nothing is sent to anyone, but anyone who sees your home screen also sees what it shows. No widget is added without you, and removing it from the home screen is enough to show nothing.

## What can leave your phone

### Subscription

The first launch, up to the making of your program, is free. After that, Reforge opens with a monthly or yearly subscription sold by Google Play, with a free trial the first time. Payment, billing, renewal, cancellation and refunds go through Google Play, under Google's terms and privacy policy: Reforge sees neither how you pay nor your Google account.

- **On your phone**, Reforge asks Google Play whether a subscription is running (at launch, and when you come back to the app), and keeps the date of the last yes, or the fact that the last answer was "no subscription". This lets it open for 3 days when Google Play can't answer, and stop the training reminders once the subscription has ended. This stays on the phone, out of the backups.
- **At the developer's**, as for any sale on Google Play, the Google Play console shows the orders (number, offer, price, taxes, country, history), so that they can be refunded or cancelled if you ask. The developer never receives your payment information.
- **Without a subscription**, the subscription screen keeps "Export my data" and "Save my photos": your data stays yours.

### Exercise illustrations

When you open an exercise's page or a session's tips, Reforge downloads its illustrations from the server of [RepDB](https://repdb.co) (`exercise-dataset.com`), then keeps them on the phone. Like any web request, this reveals the exercise viewed and your IP address. RepDB receives nothing else.

### The coach's AI

The AI is optional and off until you turn it on: at the end of the first launch, in Settings › Artificial intelligence, or with the coach's "Turn on the AI" button. A screen first says what it does and where what you write goes. You don't choose the model and have no key to enter: Reforge uses Gemini Nano if your phone can run it, and Reforge's cloud otherwise.

- **Gemini Nano (on the phone)**, if your phone can run it (Pixel 9 and 10, among others): the text is processed by your phone and nothing you write is sent. The model is downloaded by the phone's Google services (AICore), not by Reforge, and the cloud never takes over during that download. Gemini Nano doesn't read photos: estimating a meal from a photo isn't offered in that case.
- **Reforge's cloud**, if your phone can't run Gemini Nano and your version includes it: to answer you, your messages to the coach, your notes, the meals you have estimated (description, list or photo) and a summary of your profile, training and nutrition (sex, age, height, weight and body fat trend, sensitive areas, program, latest sessions, logged meals, the day's targets, diet, allergies and foods to avoid if you entered them, activity read from Health Connect if syncing is on, local date and time) are sent to Google's Gemini API, through the developer's Firebase service. This is the API's paid tier: Google doesn't use this content to train its models. Google keeps your messages and the answers for a limited time, only to detect uses its policies forbid, and this data may be stored or cached in any country where Google or its agents have facilities: this API only offers global access to its models, and the developer can't choose the region where your request is processed. Google also receives technical information (token counts, errors, device or token identifiers, IP address), which it handles under its own privacy rules. The developer neither reads nor keeps these exchanges. This cloud is for people aged 18 and over: Reforge asks you to confirm it before turning it on, and doesn't offer it if your profile's year of birth says you are under 18. A technical token (Firebase App Check, Play Integrity) goes with the requests so that Google can check they come from the official app and limit abuse. Nothing is sent until you have turned the AI on, and then until you write to the coach or have a meal estimated.
- **No AI**: while it is off, or if neither Gemini Nano nor Reforge's cloud is available, the coach answers from its knowledge base, offline.

The screen shown before turning it on says which of the two answers on your phone, and what is sent when it is the cloud. A backup (the export file, or Android's when you change phones) never turns the AI back on: you turn it on on each phone. Loads and progressions are always worked out by Reforge's rules on your phone, never by the AI.

### Products found by their barcode

When you look up a packaged product by its barcode ("Barcode" in the Nutrition tab), Reforge sends that code, and only that code, to [Open Food Facts](https://world.openfoodfacts.org), an open database run by a non-profit, to receive the nutrition facts and allergens on its label. The request contains neither your profile, nor your meals, nor any identifier; as with any connection, Open Food Facts' server sees your phone's IP address. The values received become a meal that you check before saving it, on your phone.

The code is read by the Google Play services barcode scanner (Google code scanner, ML Kit): the camera opens in those services, which give Reforge only the code read, without going through Reforge's "Camera" permission. Google says the image is analyzed on the phone. You can also type the code by hand.

### Health Connect

It is optional and off by default: at the first launch, once your program is ready and your subscription taken, Reforge offers it (you can answer "Later"), and you can turn it on later in the settings. If you do, Reforge **writes** each finished session to Health Connect (strength training session: date, duration, name, exercises) with the energy it estimates the session burned (active calories, about 3 METs above rest for the session's duration), unless your watch or another app already recorded some for that time: its measurement then wins, and Reforge adds nothing or removes its estimate; it **reads** your weight and body fat to complete your curve, and **reads** your activity over the last 7 days (steps, active calories, activities recorded by other apps) when the coach or the Nutrition tab need it, without keeping it. This data is managed by Health Connect, on your phone: Reforge sends it to no one, except the weight and body fat trend and the recent activity that go with your questions when the AI goes through the cloud. When you delete a session in Reforge, Reforge also deletes, in Health Connect, the session and the energy it had written there (never the measurements of a watch or another app). You can withdraw these permissions at any time in Health Connect.

### Technical information sent to Google

Reforge relies on three Google libraries that may send Google technical information, unrelated to what you enter in the app:

- **ML Kit**, for Gemini Nano on the phone: operating and performance metrics, with information about the device and the app (app version, phone model, Android version). They may be sent as soon as the app asks your phone whether Gemini Nano is available, so at every launch, even with the AI off.
- **Firebase**, only if you use Reforge's cloud: information about the app (its version, the library's version, its Firebase identifier) and a Play Integrity attestation token (Firebase App Check) that lets Google check the request comes from the official app.
- **Google Play Billing**, for the subscription: information about its own working (calls that succeed or fail, connection to the Google Play service).

This information is used to run, diagnose and protect these Google services. Reforge receives none of it and can't see it. The details are in Google's documentation for [ML Kit](https://developers.google.com/ml-kit/android-data-disclosure) and [Firebase](https://firebase.google.com/docs/android/play-data-disclosure).

### Reporting a coach's answer

If you report an AI answer, Reforge prepares a message (the reported answer, the reason, your comment if any, the app's version and the model used) that you review in your email app before sending it to the developer. Nothing is sent without your consent, and this message contains neither your profile nor your sessions.

### Backups and exports

- If Android backup is on for your phone, Android may back up Reforge's data (database and settings) to your Google account, according to your Android settings.
- "Export my data" (in the settings, and on the subscription screen) creates a JSON file that you save wherever you want: Reforge keeps no copy of it.
- "Automatic backup" is off until you choose a folder in Android's picker (on the phone, a memory card, or a cloud whose app offers it). Reforge then writes the same file as an export there, after each session and once a day, and keeps the last 7; it can only reach that folder, not the rest of the storage. If the folder is synced with a cloud, it is that cloud's app that uploads the file, not Reforge. Stopping it gives the folder's access back, and the files already written stay there.

## What Reforge doesn't do

Reforge shows no ads, doesn't measure your use, builds no advertising profile, contains no ad tracker or analytics tool, and neither sells nor shares your data with third parties.

## Android permissions

- **Internet**: download the illustrations, look up a product in Open Food Facts by its barcode, and reach the AI in the cloud when you turned it on on a phone that can't run Gemini Nano.
- **Google Play billing**: subscribe and check your subscription, through the phone's Google Play app.
- **Notifications, vibration, exact alarms**: tell you when the rest time is over, even with the screen off.
- **Training reminders** (optional, off until you turn them on): a notification on the days a session is planned, made on your phone from your program and sessions, without sending anything to anyone. Android asks you for the notification permission when you turn them on, and the "Training reminders" category in its notification settings lets you mute them. Reforge sets the next reminder's alarm again when the phone restarts ("Run at startup" permission, harmless: it gives access to nothing).
- **Health Connect** (writing sessions and their energy; reading weight, body fat, steps, active calories and activities): optional, see above.
- **Camera** (optional): Android asks you the first time you take a photo from Reforge. It is used to take your photos with Reforge's camera: a meal always on the back lens, a progress photo on the lens of your choice, with a timer if you want one. If Reforge's camera can't open, your camera app takes over (Android lets an app that has its own camera open the phone's camera app only with this permission). Reforge only uses the camera while its camera screen is open, and the image follows the path described above: never kept for a meal, kept on the phone only for a progress photo. If you refuse, you can still choose a photo from your gallery.
- **Barcodes**: the Google Play services scanner opens its own camera and gives Reforge only the code read; it doesn't use Reforge's "Camera" permission.
- **Gallery**: Reforge doesn't ask for access to your photos: Android's photo picker gives it only the photo chosen.

## Your choices

- Change or cancel your subscription: Settings › My subscription, or in Google Play (Payments & subscriptions). Once cancelled, it stays active until the end of the period paid for; cancelled during the free trial, it costs nothing.
- Turn the AI on or off: Settings › Artificial intelligence (or "Turn on the AI" in the coach).
- Enter, change or clear your diet and allergies: Nutrition tab or Settings › Food › Diet and allergies ("Clear all").
- Turn on, set or mute training reminders: Settings › Training reminders, or the "Training reminders" category in Android's notification settings.
- Withdraw Health Connect permissions: in Health Connect.
- Withdraw camera access: Android's settings (Apps › Reforge › Permissions).
- Delete a session: Progress › History › the session › trash can. It is also removed from Health Connect.
- Export or import a backup, choose or stop the automatic backup: Settings › Data.
- Stop showing your data on the home screen: remove the widget, with a long press on it.
- Delete everything: uninstall the app, or clear its storage in Android's settings (Apps › Reforge › Storage). Sessions written to Health Connect stay there: delete them in Health Connect, or one by one in Reforge before uninstalling it (deleting a session in Reforge also removes it from Health Connect).

Apart from the orders Google Play shows them, the developer holds no data about you: for a question about your subscription or a refund, write to them or go through Google Play. For what is sent to Google (subscription, cloud AI when turned on), your rights are exercised with Google.

## Health

Reforge gives training and nutrition guidance; it is not medical advice. If you have pain, an injury, are pregnant or ill, ask a health professional before training. The allergy filter leaves out the foods in its table that usually contain the allergen, but it knows neither traces, nor processed products, nor restaurant dishes: it replaces neither reading labels nor the advice of an allergist or a doctor.

## Children

Reforge is not meant for children and collects no data about them.

## Changes

When this policy changes, the date at the top of the page changes too, and important changes are announced in the release notes.

## Contact

A question about this policy? Write to [nvong.dev@gmail.com](mailto:nvong.dev@gmail.com).
