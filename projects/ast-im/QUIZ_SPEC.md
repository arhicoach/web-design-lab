# Current quiz / lead workflow — preserve, do not rebuild blindly

Existing Flexbe page-local quiz modal: quiz21012. First: property type. Second: area. Third: engineering systems multi-select. Fourth: preferred contact method. Contact branches (current, superseding 2026-11-07 instruction):
- Call by phone → step qphone20261107, placeholder “Введите номер телефона”
- WhatsApp → qwa20261107, “Введите номер телефона”
- Telegram → qtg20261107, “Введите номер телефона или аккаунт Telegram”
- MAX → qmax20261107, “Введите номер телефона”

Choice step q9b56ef8b routes via vars[].goto. Prior inspection revealed possible stale choice.child = [qa88a9e53] pointing to removed shared contact step: **verify graph consistency and actual end-to-end navigation before production**. Do not assert tested.

Quiz submit redirects to existing https://ast-im.ru/thankyoupage/ (pageId 1491307); do not edit thank-you page. Other local engineer form modal done88421 exists; preserve/test it. Check required fields, privacy consent, notifications, actual lead delivery and thank-you redirect before publishing. Do not fake form submissions or success.

CTA buttons should open existing quiz, not a disconnected demo form. For standalone prototype, demonstrate quiz trigger with explicit “integration pending” if real integration unavailable.
