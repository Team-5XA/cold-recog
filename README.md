<div align=center>
  <img src="https://media-hosting.imagekit.io//97787fca7ac24cda/5XA.png?Expires=1834548660&Key-Pair-Id=K2ZIVPTIP2VGHC&Signature=u5AothZchaTsjbTJfePDefGjRPX1feaKTBZ96ePdkLb2Lbc3TG27IViOwFT0tQtx29xIZNUZJSe88Y~KjSdWkPHRq3fABY4arZRarHNJaELUh3jhQYo2QXu3I3zv8gG5PfeF5Qp-GGbX8PqgWKqcUr8SGjIdkPymWaIhlo0M-bOtyHGyeuHlYNO6CUx8hzmXDFvdiNzLyUbpdrsfkodexFbrb6RLzmkcMxJqXtUJljuB8uVQ1VPcb8htSw~~cwg3N7D3EPpAjd9KiYlPdXdLthKWqsp0XL5QUnRO2D7xr1jPdFMQPOEXO8JbuhXA1DPzpLwDKDU8UqeDavmkcWc0WQ__" width="137" alt="Logo" />
       &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <img src="https://media-hosting.imagekit.io//696d072a6b054e3d/swappy-20250219-102605.png?Expires=1834549008&Key-Pair-Id=K2ZIVPTIP2VGHC&Signature=eAI71jIbkQGpe4KoiraHwokpDPK~QpJrnwauWgrWrbSU6gk4-MqFtsEDf9HltzsitvZQN8D6RDVkuZmt06M~gMSUV0bT68MSc0cgTqxyvlrb-NvwgJtcCRWBMNZQXS7TOmCqocy9aNb0~1Dj0UvFH6PZMPZxPUstbD-x~15smPNbvXKhZVYsObcLfthECsV4LW3F5K6f~tvrglJZM64wHQ0OCkrW6tDh3X2uEUDsfgyAAP29mFNH8JtUlsbOEtSrzCxGjABv3bTPPqcSnwy72WyM-vIESHNXBEBsdtEMCdpT1O7Q8P2a4OrZSLtTahYyDOz6txNCfEscyfziX4L5Mw__" width="215" alt="Logo" />
</div>

# Cold-Recog 📇 - IDENTIFICATION OF UNIDENTIFIED PERSON USING IDENTITY CARD 

###  What is Cold-Recog ❓

**Cold-Recog** (COLD: Corpse Or Lost Deceased, RECOG: Recognition) – An system for the identification of deceased or missing persons)



## [Check out our demo video ✌🏽](https://youtu.be/9FdiVLZ_B7U)


# Table of Contents

- [Reason](#reason)
- [Features](#features)
- [Architecture](#architecture)
- [Usage](#usage)
- [Research](#research)
- [License](#license)


# Reason 

Countless bodies remain `unidentified`, leaving families in endless grief while NGOs and authorities struggle to trace their identities. 💔 `DNA testing` costs ₹50,000–₹60,000 and takes weeks—far too long for those desperate for answers. `ColdRecog` was born from this `pain—a hope`, a solution, a way to reunite names with the lost. No one deserves to be forgotten. 🕊️

# Features 
✅ <b>Automated Facial Recognition</b> – Uses deep learning-based `facial detection` to match unidentified corpses with government-issued ID images.

✅ <b>AI-Powered Identity Verification</b> – Implements `TensorFlow` and advanced image processing techniques to enhance matching accuracy.

✅ <b>Secure Authentication</b> – Uses `JWT-based authentication` for secure access to the platform.

✅ <b>Multi-Platform Support</b> – Available as a `React`-based web app and a mobile app `(Expo-based for Android & iOS)` for seamless access.

✅ <b>Document Matching & Vectorization</b> – Extracts and verifies identity documents (Aadhaar, voter ID, driving license) using API-based validation and vectorization techniques.

✅ <b>REST API Integration</b> – Efficiently communicates with the backend `(Flask-based server)` via `RESTful APIs` for processing and data retrieval.

✅ <b>Scalable & Secure Database</b> – Stores and manages `identity data` securely for accurate matching and retrieval




# Architecture 

 <img src="https://media-hosting.imagekit.io//d430385ee5774386/Document%20verification.svg?Expires=1834550622&Key-Pair-Id=K2ZIVPTIP2VGHC&Signature=Pd81HlsLof18da9jU2cYbbErt4NApi2kC2lO6ENkMhRGU0d2tYqKwEBZ7Or6qbQ5TX7NSNuHThLCKrYRPexWfRKQIC5LeWgWAvRIKTAunvUstVIYBiOtMeIN0V94FqP5NpijSp2gbpJrtB1E5k-cO~2k8bLgROBF1CUXpqfxXAic-9JZ8DiMRScBfhJNwu8kERYxvmYUfA7Fq6lZHDu2eGqJosxunTenFWJJcKXfdJ1Vp~IiWKI1SPayrQfTED2hSA75~I3l69qB3wtx0ObRMXegG57EHq2g3cSW5x5Phx3ypg6jEvby-knbn0eRy1n3aapm3peip6fkwmhESJNNUA__" width="900" alt="Logo" />


Cold Recog is designed to assist in identifying unidentified bodies by comparing facial images with an `Aadhaar image database` using advanced image comparison techniques. The system architecture consists of the following components:

1. <b>Web & Mobile Applications</b>

  The system provides both a `web and mobile interface` for users to interact with the platform.
  The web app (built with React) and mobile app (developed using Expo) allow users to `authenticate`, `upload images`, and `view results`.

2. <b>Authentication</b>

    Users must log in via the `JWT authentication` system to securely access the platform.
    Authentication is necessary for accessing the image upload and verification features.

3. <b>Image Upload & Capture</b>

    Users can `upload images or capture` them using their mobile devices.
    The uploaded images are then sent to the `backend` for processing.

4. <b>Server & Database (Document Verification & Face Recognition)</b>

    The backend, built using `Flask`, handles the core image processing and `facial recognition` tasks.
    TensorFlow is used for facial detection and feature extraction.
    Document verification involves:
        Facial detection to extract and validate the face from the uploaded image.
        Compatibility check to compare the extracted face with database images.
        Vectorization of images for efficient comparison.
        API checks to verify additional document details.

5. <b>Result Display</b>

    The system provides `results` through both the `web app and mobile app`, displaying matching or potential matches from the database.


# Usage

To view the full usage of the project, please click the link below.  
It will lead to the `HOWTOUSE.md` file.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;

<a href="/HOWTOUSE.md"><img src="https://media-hosting.imagekit.io//9f182a17d5464129/cr.png?Expires=1834924181&Key-Pair-Id=K2ZIVPTIP2VGHC&Signature=mFwVsRkz7AkJKrHJC8GQbSCLqmUObcY~DxCSSc07BgTUw1ow2fg2EqP4ksYir6OXGe9SH6tXfFYKgE5C7Ka9mSSf4y2Go2-UuehdXFdRGbnIOq0UFM2d7tIlyfFS~k9XM8nyJnsf7aVa--E2F-uRKA-3HQf1rX73kiiLIKYM1RW0DoTCDp2gkWrdwcbXCv1rAcjpzVf0hdWe5e1-Xhh0R20SNnvzYqL7ZR831J8tiWCj2gAm~-YdoPDmwdc80dFLgI~JYbPyZdIZ8hrL4o7hHhtrcLIINZaLIcEV4zp4rt9kPKBsTs1-w-bHZ7dZD9bX6WcwwPgO08GW~Bl1JXQbyA__"></a>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;

# Research 
<div align=center>
 <img src="https://media-hosting.imagekit.io//97787fca7ac24cda/5XA.png?Expires=1834548660&Key-Pair-Id=K2ZIVPTIP2VGHC&Signature=u5AothZchaTsjbTJfePDefGjRPX1feaKTBZ96ePdkLb2Lbc3TG27IViOwFT0tQtx29xIZNUZJSe88Y~KjSdWkPHRq3fABY4arZRarHNJaELUh3jhQYo2QXu3I3zv8gG5PfeF5Qp-GGbX8PqgWKqcUr8SGjIdkPymWaIhlo0M-bOtyHGyeuHlYNO6CUx8hzmXDFvdiNzLyUbpdrsfkodexFbrb6RLzmkcMxJqXtUJljuB8uVQ1VPcb8htSw~~cwg3N7D3EPpAjd9KiYlPdXdLthKWqsp0XL5QUnRO2D7xr1jPdFMQPOEXO8JbuhXA1DPzpLwDKDU8UqeDavmkcWc0WQ__" width="137" alt="Logo" />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
 <img src="https://media-hosting.imagekit.io//a9dee0bc30e8472a/uruvugal.jpg?Expires=1834575746&Key-Pair-Id=K2ZIVPTIP2VGHC&Signature=yu1yk3arqYLMACtvqZxS6hMtlu~8-hWA~UImvYqMICh3p~dGgCVgH-H7D3StpaDOZfQEj-K0HDCbFa4lyy9A07VkqyyUam-tNAcO2PfGpaL3F2t85oV2qh-4RJZfSNCmZAKf97iCCGqytWv5QABg~u2c6BACkAYesNiK-ngaHSZbASlhUQlgavyVjEZlYw3~DnwzGjrTacH47geR~6NWCuHK33RxNVhJR76w3SJGQnUjEDeL39Yr2mlxopWSI9fmYAviCxu6HTaooIceRtRDkb1ePh5iX-XzhvHTmXFqvv6HN65V2GtVepdVJT2ga15EOkNPljHhM2sQIrKrlYQlTQ__" width="137" alt="Logo" />

 </div>

To advance our research, we partnered with <b>[Uravugal Trust](https://uravugaltrust.com/)</b>, a respected `NGO` that has been performing last rites for unclaimed bodies for the past three years. Their extensive experience and insights have been invaluable in shaping our approach.
Mortuary & Cremation Study

<b>`On August 28th`</b>, our team conducted fieldwork at <b>Rajiv Gandhi Government Hospital</b> to gain firsthand experience of the burial process for unclaimed bodies. This visit provided us with both an emotional perspective and a practical understanding of the challenges involved. Following this, we `visited a nearby crematorium` to further observe and study the procedures.

💡 Key Insight: According to [Uravugal Trust](https://uravugaltrust.com/), more than `80% of unclaimed bodies` are found without `facial decomposition`, making facial recognition a viable approach for identification.

# Engagement with Law Enforcement

To explore the legal and practical aspects of implementing our solution, we visited the <b>`Commissioner of Police’s office` </b>in Egmore. During a two-hour meeting, we presented our project to <b>M.S. Bhaskar, Assistant Commissioner of Police (Greater Chennai Corporation)</b>.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img src="https://media-hosting.imagekit.io//cb99680d6f874ba0/swappy-20250219-174511.png?Expires=1834575338&Key-Pair-Id=K2ZIVPTIP2VGHC&Signature=O8U264eHavUEkbgg6LLXB44DrXc9vsjvT8nfoYUUSDI1cy-~tSOASUY2FDRRp3Y1kIhJYsdWqoZBeKUFkmck9u5VRC6fkX8BcFEj2KvfEI6cf~QAmD7bX-7cnZjW7bcWa8jBDq2mBZf~7b60N5~AvtnI0Ftp8SFwPf7wRKOosrOfzsRqayBjPaj8RJNfEWNqtBweFtv~~6JZsHIwzhZamtEZyY9eoVSK4TCe-XAOGJ59UjOiYgJxV-SCip43J-MJuTJQXchmRFp0WEt9fCBozfVP~~We8bT~2KuiBVxHcAY-9pbwSfaZBo32JdrFl6nzkNCvZExfpUJAwYundXe1Ng__" width="715" alt="Logo" />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;

<b>🔹 Key Takeaways from the Meeting:</b>

  - `Mr. Bhaskar` expressed strong support for our initiative.
  - He advised starting with `voter ID verification` to test the feasibility of our solution before expanding to other ID databases.
  - His feedback helped refine our approach, ensuring alignment with law enforcement protocols.

# Team Behind COLD-RECOG
### Team Name: 5XA

#### Team Members : 

- **B A Aksshay**: [GitHub Profile](https://github.com/aksshay88)
- **Abhishek Renjan U B**: [GitHub Profile](https://github.com/Ren-Gen22)
- **Aakash S**: [GitHub Profile](https://github.com/Aak54321)
- **B A Aswin**: [GitHub Profile](https://github.com/aswin8846)

# Contribution

We welcome contributions and feedback from the community to enhance our  solution. Your insights are invaluable in shaping the future of this project. 

- **Contributions**: We encourage developers to contribute code, documentation, and ideas to improve functionality and usability.
- **Feedback**: Please share your thoughts and experiences to help us identify areas for improvement and feature enhancements.
- **Issue Reporting**: If you encounter any issues, we invite you to raise them through our issue tracker, ensuring that we can address them promptly.

Together, we can create a more robust and effective solution for the society .

# License

This project is licensed under the MIT License. You are free to use, modify, and distribute this software under the terms of the [MIT LICENSE](https://github.com/Team-5XA/cold-recog/blob/main/LICENSE)
