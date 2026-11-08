# bRide Privacy Policy

**Effective date:** [TBD — date of publication]

bRide is a workplace attendance application provided by HumbleBeeAI for authorized organizations and team members. This Privacy Policy explains what information bRide processes, why it is processed, and the choices available to users.

## 1. Information bRide processes

### Account and employee information

When you sign in through HStaff, bRide may receive information associated with your authorized employee account, such as your name, work email, profile photo, role, assigned branch, timezone, work schedule, day-off request count, and approved work or social connections.

### Attendance information

bRide processes attendance-related information such as check-in events, AFK periods, planned return times, optional AFK reasons, late-arrival reasons and estimated arrival times, full-day-out reasons, workday completion, office assignment, and related timestamps.

### Location information

bRide collects location only to decide whether you are at an approved office. It does not track your route, record where you are outside the office, or build a map history of your day.

**How it works.** After you sign in and grant permission, your phone places an invisible circle (geofence) around each approved office. The phone's operating system watches these circles; bRide is not running and reads no location while you are away from an office. When you enter or leave a circle, the phone wakes bRide, which turns on GPS for a short time (seconds, at most about 10 minutes while you approach) to confirm the event, then turns GPS off again. Because the phone is usually in your pocket, this requires "Always" location permission and precise location.

**What is sent to the server and stored:**

| When | What is stored | Coordinates? |
|---|---|---|
| Office check-in (manual button or automatic on arrival) and, optionally, returning from AFK | Time, office, latitude/longitude of 1–3 GPS readings taken at the office, GPS accuracy, distance from the office, verification result | **Yes**, as check-in evidence |
| Entering or leaving an office during the day | Time, office, enter/exit, distance from the office (meters), GPS accuracy | **No** |
| Arrival recorded while the server was unreachable | Arrival time only | No |
| Location setting status | Whether "Always" location, precise location, and (iOS) Background App Refresh are on | No |
| Remote check-in, late reason, full-day-out | Reason text and time | No (location not used) |

Manual office check-in requires a current GPS reading to confirm you are at the office. Remote check-in does not use location.

**When.** Location is checked only when you check in or when your phone enters or leaves an office circle. It is not checked on a timer. bRide sends nothing while you are away from all offices, including at home, outside working hours, during breaks, and on days off. If you pass through an office circle outside working hours, during a break, or on a day off, the entry or exit is still recorded, but no reminders are sent and, on days off, it is not counted for lateness, AFK, or early-departure statistics. On remote days office entries and exits are not stored. Signing out removes all office circles, and bRide can no longer wake up.

If the server cannot be reached, confirmed entry and exit records are kept on your phone for up to 7 days and sent when the connection returns.

**Who can see it.**

- Authorized administrators of your organization see, in the attendance dashboard, your check-in time, out time, AFK periods, office entry and exit times (up to the last 31 days at a time), and whether your location settings are off. The dashboard does not show coordinates, distances, or maps.
- Check-in coordinates are kept as evidence on the server and are not shown in the dashboard. They are accessible only to service operators for verification, troubleshooting, and dispute resolution.
- Discord attendance messages contain only short status texts (for example `in-09:02`, `afk-13:00`, `back`, `done`) and never contain coordinates.

bRide does not use location for advertising and does not sell or share location with third parties for their own purposes.

**Consent.** bRide collects location only after you give consent and grant the location permission on your device. You can withdraw consent at any time by turning off location permission in your device settings or by signing out. If you do, automatic check-in and office entry/exit recording stop, and your out time may be incorrect; the app will show a reminder and the dashboard will show that your location setting is off.

### Announcements and read status

bRide may retrieve announcements available to your HStaff account and process whether an announcement has been read so the Inbox can display accurate unread status.

### Device and app information

bRide may process limited technical information needed to operate securely and reliably, such as app version, notification permission state, geofence registration state, request identifiers used to prevent duplicate attendance events, and diagnostic errors. Authentication tokens are stored using the device’s secure storage facilities.

## 2. How information is used

Information is processed to:

- authenticate your authorized account and restore your session;
- show your employee profile, schedule, and announcements;
- validate office attendance and maintain accurate workday status;
- prevent duplicate attendance updates;
- send relevant local notifications and reminders;
- deliver approved attendance updates to organization-authorized Discord destinations; and
- protect, troubleshoot, and improve the reliability of the service.

## 3. Where information is processed and stored

The mobile app communicates only with the bRide server. The bRide server and its PostgreSQL database are hosted by [TBD — cloud provider] in [TBD — region, e.g. Seoul, Republic of Korea]. All location and attendance records are stored there.

The bRide server retrieves authorized profile, schedule, and announcement data from HStaff, and may deliver attendance status messages to an organization-approved Discord channel or thread. Discord is operated by Discord Inc. in the United States; only the short status texts described above are sent to it, never location data.

The mobile app does not directly connect to HStaff, PostgreSQL, or Discord for attendance operations.

## 4. Sharing of information

Information may be available to:

- your organization and authorized administrators;
- service operators who maintain bRide and HStaff;
- infrastructure providers used to host and secure the service; and
- Discord, when your organization has enabled attendance status delivery.

bRide does not sell personal information and does not use attendance or location information for targeted advertising.

## 5. Retention

| Data | Kept on the server for |
|---|---|
| Check-in location evidence (coordinates) | [TBD — e.g. 6 months] |
| Office entry/exit records | [TBD — e.g. 1 year] |
| Attendance records (check-in, AFK, out times, reasons) | [TBD — e.g. 3 years, or as required by labor law] |
| Location setting status | Until replaced by the next update |

When the retention period ends, or when you leave the organization and the records are no longer needed, the data is deleted. Data may be kept longer only where a law requires it. Confirmed entry/exit records waiting to upload are deleted from your phone after 7 days.

Local app data, including secure session credentials and cached profile or attendance context, is removed or invalidated when you sign out. Some device-managed secure storage may follow operating-system backup or keychain behavior.

## 6. Security

bRide uses measures designed to protect information, including encrypted HTTPS connections, secure device storage for authentication tokens, authenticated API access, server-side attendance validation, access controls, and duplicate-request protection. No security measure can guarantee absolute protection.

## 7. Your choices and rights

You can control location and notification permissions in your device settings. Disabling precise or background location may prevent automatic check-in, geofence monitoring, and office-exit reminders from working.

Depending on your location and your organization’s policies, you may be able to request access to, correction of, or deletion of personal information. Contact your organization administrator first for employment-related records. You may also contact HumbleBeeAI using the details below.

## 8. International processing

bRide, HStaff, hosting providers, or Discord may process information in countries other than the country where you work. Appropriate organizational and technical safeguards should be applied based on the deploying organization’s requirements and applicable law.

## 9. Children’s privacy

bRide is a workplace application for authorized team members and is not directed to children under 13. It should not be used by anyone who is not eligible for an authorized employee account.

## 10. Changes to this policy

This policy may be updated when bRide’s features, service providers, or legal requirements change. The effective date above will be updated when a revised policy is published.

## 11. Contact

**HumbleBeeAI**  
76, Gyeonginnam-gil, Michuhol-gu, Incheon, Republic of Korea  
Email: [support@humblebee.ai](mailto:support@humblebee.ai)  
Website: [https://www.humblebee.ai/](https://www.humblebee.ai/)

