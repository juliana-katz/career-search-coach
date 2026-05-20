# How to export your LinkedIn connections

Most people haven't done this. Walk them through it patiently.

## Steps

1. Open LinkedIn (desktop browser is easier than mobile)
2. Click your profile photo (**Me**) in the top-right nav
3. Click **Settings & Privacy**
4. In the left sidebar, click **Data Privacy**
5. Under "How LinkedIn uses your data," click **Get a copy of your data**
6. Select the radio button **"Want something in particular? Select the data files you're most interested in"**
7. Check ONLY the **Connections** box (not the full archive — that takes 24 hours)
8. Click **Request archive**
9. LinkedIn will email you a download link within 10 minutes (sometimes up to 30 min)
10. Click the link in the email → download the zip
11. Unzip → find **`Connections.csv`**
12. Note the full file path — share that with Claude

## What's in the CSV

7 columns:
- First Name
- Last Name
- URL (their LinkedIn profile URL)
- Email Address (only if they've opted to share)
- Company (current employer)
- Position (current title)
- Connected On (date)

## Privacy note

The CSV stays on the user's machine. Claude reads it locally to find matches at target companies. Don't share the file with third parties.

## Bonus: spouse/partner export

If the user's spouse, partner, or close friend has a complementary network and is willing to share, they can run the same export. Two CSVs roughly doubles the warm-contact surface area. Be respectful — only ask if the user volunteers this.

## Failure modes

- **Can't find "Get a copy of your data"** — LinkedIn occasionally redesigns the privacy settings page. The user can search "data export" in LinkedIn's help center.
- **Email never arrives** — Check spam folder. If still nothing after 1 hour, request the archive again.
- **Connections.csv is empty or near-empty** — User likely has a private profile or hasn't connected with many people. The skill still works (focus more on cold outreach + 2nd-degree paths) but warm-contact discovery is limited.
