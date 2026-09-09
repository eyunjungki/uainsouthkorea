UAinSouthKorea.com — website files
==================================

WHAT'S HERE
  index.html          the whole site (one page)
  images/2026/        the 2026 cohort's photos
  images/2025/        the 2025 cohort's photos
  images/trip-poster.jpg   the still shown before the video plays
  trip-video.mp4      the trip film, compressed for the web (14 MB)

PUBLISH IT (free, about 10 minutes)
  1. Go to https://pages.cloudflare.com and sign in (free account).
  2. Create a project > "Upload assets" (Direct Upload).
  3. Drag this whole folder in. It goes live at something like
     ua-in-south-korea.pages.dev.

CONNECT UAinSouthKorea.com (bought at Namecheap)
  4. In the Cloudflare Pages project: Custom domains > Set up a domain >
     type uainsouthkorea.com. Cloudflare shows the DNS records to add.
  5. In Namecheap: Domain List > Manage > Advanced DNS. Delete Namecheap's
     default parking-page records, then add the records Cloudflare gave you.
  6. Wait 10-60 minutes. HTTPS is issued automatically and is free.

UPDATING IT EACH YEAR
  Open index.html and scroll to the bottom. Two lists are marked
  "EDIT HERE EACH YEAR":

  PHOTOS   Make a folder images/2027/ and copy the new pictures in.
           Then add a block at the TOP of the GALLERY list:

             {
               year: "2027",
               note: "Summer 2027 &middot; Seoul, Gyeonggi, Gangwon, Jeju",
               photos: [
                 { src: "images/2027/somephoto.jpg", cap: "Short caption" },
                 { src: "images/2027/another.jpg",   cap: "Short caption" }
               ]
             },

  QUOTES   Add a new entry at the top of the TESTIMONIALS list:

             { text: "What the student wrote.",
               name: "Their name or @handle",
               role: "Major, UA &middot; LinkedIn" },

  Everything else (dates, courses, itinerary) is plain text in the page —
  search index.html for the words you want to change.

REPLACING THE VIDEO
  Keep the file under 25 MB (Cloudflare's per-file limit) and name it
  trip-video.mp4 so no code has to change.
