# TestData

🧾 避難者登録（User Registration） – Full Breakdown
Based on the PPT, there are 4 main registration methods in the system:

📱 1. スマホによる登録 (Smartphone Pre-registration)
Evacuees can scan a QRコード on the municipal website or a poster in the shelter.

They fill in the following on their own device:

氏名 (Name), 住所 (Address via postal code auto-fill), 生年月日, 性別

要配慮者情報 (Special needs), 体調 (Health condition)

自宅の居住可否 (Habitable or not)

個人情報の取り扱いに同意 (Check required)

公開情報の可否 (Optional)

Upon completion:

A QRコード付き登録画面 is shown.

Evacuees can download/save this QR and bring it to the shelter for final admission.

💳 2. 身分証（マイナンバーカード・運転免許証）による登録
Staff uses a スキャナー to scan printed info on ID cards.

Process:

Click 新規登録

Select the number of evacuees

Click 身分証スキャン and place the card correctly

Data is read (Name, DOB, Address auto-filled)

Add remaining data (Gender, Health info, Support needs)

Review → 同意チェック → 登録

Generates a 管理番号, needed for退所

Multiple evacuees in a household can be entered consecutively

📄 3. QRコードによる登録
For users who already have a pre-issued QRカード with personal info

Process:

Click 新規登録

Click QRスキャン

Use ハンディスキャナー about 10cm from the card

Name, phone, address auto-fill

Continue with health/support data

同意 → 確認 → 登録

🧍 4. 手動入力 (Manual Input by Staff)
Used if evacuee has no ID/QR or technical issue occurs

Staff manually inputs all fields:

Name, Address, DOB, Phone, Gender, Health/Support details

This method is accessible via:

新規登録 button in the スタッフ画面

Follows same flow as other methods (review, consent, confirm)

📌 After Registration
The evacuee appears in the 避難者一覧

Staff can view or edit their profile

退所処理 can be done later via 退所手続き
below are page urls
const pageTitles_en = {
        // Admin URLs  
        "/admin/login": "Admin - Login",
        "/admin/dashboard": "Admin - Dashboard",
        "/admin/settings": "Admin - Settings",
        "/admin/event-status-list": "Admin - Event-Status-List",
        "/admin/event-attendees-list": "Admin - Event-Attendees-List",
        "/admin/history/place": "Admin - History Place",
        "/admin/evacuation": "Admin - Evacuation",
        "/admin/temp-registration": "Admin - Temp Registration",
        "/admin/external/family/list": "Admin - External Family List",
        "/admin/shortage-supplies": "Admin - Shortage Supplies",
        "/admin/stockpile/summary": "Admin - Stockpile Summary",
        "/admin/statistics": "Admin - Statistics",
        "/admin/qrcode/csv/import": "Admin - QR Code CSV Import",
        "/admin/staff-management": "Admin - Staff Management",
        "/admin/hq-staff-management": "Admin - HQ Staff Management",
        "/admin/admin-management": "Admin - Admin Management",
        "/admin/event": "Admin - Event",
        "/admin/questionnaire": "Admin- Questionnaire",
        "/admin/place": "Admin - Place",
        "/admin/material": "Admin - Material",
        "/admin/stockpile/master": "Admin - Stockpile Master",
        "/admin/special/care": "Admin - Special Care",
        "/admin/setting": "Admin - Setting",
        "/admin/event-attendees-list/family-detail": "Admin - Event Attendees Family Detail",
        "/admin/evacuation/family-detail": "Admin - Evacuation Family Detail",
        "/admin/temp-registration/family-detail": "Admin - Temporary Registration Family Detail",
        "/admin/external/family/list/family-detail": "Admin - External Family List Detail",
        "/admin/place/create": "Admin- Create Place",
        "/admin/place/detail": "Admin - Place Detail",
        "/admin/place/edit": "Admin - Place Edit",
        "/admin/external/family": "Admin-External Evacuee Summary",
        "/admin/questionnaire/master": "Admin-Master Questionnaires",
        "/admin/questionnaire/individual": "Admin-Individual Questionnaires",

        // User URLs  
        "/user/list": "Place List",
        "/user/dashboard": "User Dashboard",
        "/user/register/member": "Register Member",
        "/user/register/member/details": "Register Member Details",
        "/user/checkout": "Checkout",
        "/user/checkout/details": "Checkout Details",
        "/user/external": "External",
        "/user/public-evacuees/": "Public Evacuees",
        "/user/temp-register": "Temporary Registration",
        "//user/temp-edit/confirm": "Temporary Details Confirmation",
        "/user/temp-register/success": "Temporary Registration Success",
        "/user/temp-edit": "Temporary Edit",
        "/user/person-count": "Person Count",
        "/user/event-list": "Event List",
        "/user/event-list/": "Event List",
        "/user/event/dashboard": "Event Dashboard",
        "/user/event/register": "Event Register",
        "/user/event/register/member": "Event Register Member",
        "/user/event/register/member/details": "Event Register Member Details",
        "/user/event/checkout": "Event Checkout",
        "/user/event-checkout/details": "Event Checkout Details",
        "/user/qr/app": "QRCode Scan",
        "/event/register/member/success": "Event Register Member Success",
        "/user/event/register/member/success" : "Event Registration Success",
        "/user/qr/app/place-list": "Place List",
        "/user/temp-edit/confirm" : "Pre-evacuation Evacuee Edit Confirmation",


        // Staff URLs  
        "/staff/login": "Staff - Login",
        "/staff/dashboard": "Staff - Staff Dashboard",
        "/staff/family": "Staff - Staff Family",
        "/staff/family/family-detail": "Staff - Family Detail",
        "/staff/temporary/family-detail": "Staff - Temporary Family Detail",
        "/staff/external/family-list/family-detail": "Staff - External Family List Detail",
        "/staff/temporary/family": "Staff - Temporary Family",
        "/staff/external/family-list": "Staff - External Family List",
        "/staff/stockpile/dashboard": "Staff - Stockpile Dashboard",
        "/staff/stockpile/history": "Staff - Stockpile History",
        "/staff/supplies": "Staff - Supplies",
        "/staff/register/check-in": "Staff - Register Check-in",
        "/staff/event-staff/dashboard": "Staff - Event Dashboard",
        "/staff/event-staff/family": "Staff - Event Family",
        "/staff/event-staff/family/family-detail": "Staff - Event Family Detail",

        // HQ Staff URLs  
        "/hq-staff/login": "HQ Staff - Login",
        "/hq-staff/dashboard": "HQ Staff - Dashboard",
        "/hq-staff/history/place": "HQ Staff - History Place",
        "/hq-staff/evacuation": "HQ Staff- Evacuation",
        "/hq-staff/temp-registration": "HQ Staff- Temp Registration",
        "/hq-staff/external/family/list": "HQ Staff - External Family List",
        "/hq-staff/shortage-supplies": "HQ Staff - Shortage Supplies",
        "/hq-staff/stockpile/summary": "HQ Staff - Stockpile Summary",
        "/hq-staff/statistics": "HQ Staff - Statistics",
        "/hq-staff/place": "HQ Staff - Place",
        "/hq-staff/material": "HQ Staff - Material",
        "/hq-staff/evacuation/family-detail": "HQ Staff - Evacuation Family Detail",
        "/hq-staff/temp-registration/family-detail": "HQ Staff - Temporary Registration Family Detail",
        "/hq-staff/external/family/list/family-detail": "HQ Staff - External Family List Detail",
        "/hq-staff/place/detail": "HQ Staff - Place Detail",
    };
