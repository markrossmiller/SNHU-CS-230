# SNHU-CS-230

The Gaming Room asked us to help them design a client and server application for their game, Draw It or Lose It. They wanted a server-side architecture which allows for distribution of a set of images for the purposes of creating a client-side application which places teams against each other in a battle for guessing the right concept based on the images provided.

In the documentation, I gave my input about what I think is the best architecture for both the server side as well as which platforms should be focused on first in developing a client-side application. I chose OpenBSD as my preferred server-side platform, hosted on a bare metal server, but conceded to the fact that OpenBSD is much more difficult to set up than a Linux-based platform, so for this reason I proposed Linux should be a sufficient platform.

For the client-side application, I recommended The Gaming Room to focus on Android development first, then on iOS, as these are the two most popular mobile platforms, and mobile app development is still booming, without any sign of slowing down.

On the server, I said that the image repository be cached on a tmpfs file system, which is memory based, to increase the speed by which the images can be fetched from the server. I also recommended putting money into buying hosting on a platform with high speed and plenty of bandwidth.

When we developed server-side code in Java, I found it difficult to get the code to run because of a conflict in dependencies. In order to make the (properly coded) source to run correctly, I was required to do a bit of manipulation to the source in order to satisfy said dependencies.

I considered the user’s needs when I laid out plans to cache a set of 8 images on the Android application, in order to allow a speedy access to images without much lag because of the server, while keeping the size of the running application small and to not inhabit too much of the phone’s or tablet’s storage space.

