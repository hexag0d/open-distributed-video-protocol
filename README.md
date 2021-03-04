# open-distributed-video-protocol
Standardized internet video protocol for decentralized video distribution (ODVP)

Purpose:

decentralize video hosting across multiple video hosting platforms/websites and make end user distribution of videos easy, less time consuming, client applications should consume the object and use it to apply settings and protocols into a standardized format for authentication and video processing, distribution

Objective:

Use https to retrieve JSON objects from many remote public video hosting services and parse into machine readable parameters containing all of the necessary settings for each remote service

High level implementation requirements:

  1. Each participant should maintain a JSON object in a (to be determined) standardized location on the remote host IE { https://XXXX.com/odvp.json }
  2. Client applications will make http request to user selected platforms and retrieve ODVP json object from each platform
  3. Each ODVP json object will be parsed into a standardized format, which should include parameters such as: authentication requirements, video resolution    requirements, audio/video bitrate requirements, supported formats, supported codecs, supported formats, supported metadata
  4. Client applications should be able to authenticate the user into each system and also process the video then POST the video into each available format for each video hosting platform
  5. Server applications need to ensure their endpoints accept parameters and POST requests specified by the ODVP json object

This is a rough draft starting point and subject to change
