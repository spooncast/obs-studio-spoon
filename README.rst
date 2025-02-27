OBS Studio HTTP  REST API for RTMP Streaming Setup
==================================================
In order to do RTMP broadcasting in OBS Studio, to solve the trouble of setting the stream URL and key every time, Rest API provides an interface to set these.
When the Rest API is transmitted in the method defined below in the broadcasting application, it is automatically registered in the broadcasting settings.

It is implemented to build in both the Windows Visual studio environment and the macOS/Linux environment.

Please email all questions and advice to 
simon@spoonradio.co.



Request
-------
``POST URL : http://ip_address:9028``


* Body JSON

``{"streamUrl" : "rtmp://12.32.11.99/sstted", "streamKey" : "23SDD2sss" }``


Response
--------

* Success
``{ "result" : "0" , "streamUrl" : "rtmp://12.32.11.99/sstted" , "streamKey" : "23SDD2sss" }``

* Error
``{ "result" : "1" }``


----

What is OBS Studio?
-------------------

OBS Studio is software designed for capturing, compositing, encoding,
recording, and streaming video content, efficiently.

It's distributed under the GNU General Public License v2 (or any later
version) - see the accompanying COPYING file for more details.

Quick Links
-----------

- Website: https://obsproject.com

- Help/Documentation/Guides: https://github.com/obsproject/obs-studio/wiki

- Forums: https://obsproject.com/forum/

- Build Instructions: https://github.com/obsproject/obs-studio/wiki/Install-Instructions

- Developer/API Documentation: https://obsproject.com/docs

- Donating/backing/sponsoring: https://obsproject.com/contribute

- Bug Tracker: https://github.com/obsproject/obs-studio/issues

Contributing
------------

- If you would like to help fund or sponsor the project, you can do so
  via `Patreon <https://www.patreon.com/obsproject>`_, `OpenCollective
  <https://opencollective.com/obsproject>`_, or `PayPal
  <https://www.paypal.me/obsproject>`_.  See our `contribute page
  <https://obsproject.com/contribute>`_ for more information.

- If you wish to contribute code to the project, please make sure to
  read the coding and commit guidelines:
  https://github.com/obsproject/obs-studio/blob/master/CONTRIBUTING.rst

- Developer/API documentation can be found here:
  https://obsproject.com/docs

- If you wish to contribute translations, do not submit pull requests.
  Instead, please use Crowdin.  For more information read this page:
  https://obsproject.com/wiki/How-To-Contribute-Translations-For-OBS

- Other ways to contribute are by helping people out with support on
  our forums or in our community chat.  Please limit support to topics
  you fully understand -- bad advice is worse than no advice.  When it
  comes to something that you don't fully know or understand, please
  defer to the official help or official channels.
