# Monstercat Connect API
__Please note that this is COMPLETELY UNOFICCIAL and just my findings.__

All API calls go to https://connect.monstercat.com/.

## Overview
| URL   |      HTTP Verb      |  Functionality |
|---|---|---|
| /signin                   | POST | [Signs you in]() |
| /api/catalog/release      | GET | [Returns all releases (=albums)]() |
| /api/catalog/track        | GET | [Returns all tracks]() |
| /api/playlist             | GET | [Returns all playlists of the user]() |
| /api/playlist | POST | [Create a new playlist]() |
| /api/playlist/**&lt;playlist_id&gt;** | PUT | [Add a song to a playlist]() |
| /api/self/session         | GET | [Returns information about the users]() |
| /api/self/referral-code   | GET | [Redirects you]() |
| /api/user/**&lt;user_id&gt;**/referral-code| GET | [?]() |
| /subscription/payments/**&lt;user_id&gt;** | GET | [Returns all payments of the user]() |


### /api/catalog/track

### /api/catalog/release

### /api/playlist

### /api/self/session

### /signin post
{"email": self.username.text(), "password": self.password.text()}

### playlist put
{"_id":"56290bf0ddd2cfb810eddae9","name":"Valkyrie","userId":"55fc1f7d53c399fc274c5054","deleted":false,"public":false,"tracks":[{"trackId":"53a0c93640cc048e26f848e6","releaseId":"53a897d07f9a812a0d96bbdc"},{"trackId":"542f2c17502836c00e5be117","releaseId":"542f2bac502836c00e5be116"},{"trackId":"5614507cc5df9f40201f85ed","releaseId":"561c5da57fb673586a3d2a98"},{"trackId":"56e0a83280a64c6105fcc8ec","releaseId":"57083d7e85ff0545443034e3","startTime":0}]}

### playlist post
{"name":"TESTING","tracks":[]}

https://connect.monstercat.com/subscription/payments/5641480a9eb192373d44ad16
