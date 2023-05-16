# How to Play Sound With Java - play audio file using java


In this article we will see, how can we play an audio file in pure java, here pure means, we are not going to use any external library. You can create your own music player by the help of this article. Java inbuilt libraries support only AIFC, AIFF, AU, SND and WAVE formats.
There are 2 different interfaces which can be used for this purpose Clip and SourceDataLine. In this article, we will discuss playing audio file using Clip only and see the various methods of clip. We will cover following operations:

Start.
Pause.
Resume.
Restart.
Stop
Jump to a specific position of playback.
Play Audio using Clip

Clip is a java interface available in javax.sound.sampled package and introduced in Java7.
Following steps are to be followed to play a clip object.

Create an object of AudioInputStream by using AudioSystem.getAudioInputStream(File file). AudioInputStream converts an audio file into stream.
Get a clip reference object from AudioSystem.
Stream an audio input stream from which audio data will be read into the clip by using open() method of Clip interface.
Set the required properties to the clip like frame position, loop, microsecond position.
Start the clip
In this tutorial, we'll learn how to play sound with Java. The Java Sound APIs are designed to play sounds smoothly and continuously, even very long sounds.

As part of this tutorial, we’ll play an audio file using Clip and SourceDataLine Sound APIs provided by Java. We'll also play different audio format files.

In addition, we’ll discuss the pros and cons of each API. Further, we'll see a couple of third-party Java libraries that can also play sound.
