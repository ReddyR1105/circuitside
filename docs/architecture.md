# Architecture

Flutter widgets dispatch actions to application state. Repositories bridge state to Firebase Auth, Firestore, Storage, and callable Cloud Functions. A local Dart ranker uses sanitized trip inputs. The app previews suggestions before a validated save.

The trip document holds ownership, destination, dates, currency, and budget. Subcollections hold members, protected invitations, day records, itinerary items, activities, expenses, packing, checklists and nested tasks, operation receipts, and optional recommendation metadata. The user document is private, including preference data, templates, and device tokens.

Functions verify identity and role, validate fields, apply versioned transactions, and use stable operation IDs for retries. Conflicting edits return current state. Offline views are labeled, and pending drafts are revalidated against the server when online. Storage and Firestore use membership rules. Google Places and Routes calls use server-held credentials with quotas. Seeded discovery and travel fixtures support repeatable tests.

The service plan also includes FCM for member alerts, Remote Config for freshness and transit defaults, Analytics for aggregate workflow counts, and Crashlytics for development crash verification. App Check is optional.
