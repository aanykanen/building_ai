<!-- This document is based on the markdown template for the final project of the Building AI course, 
created by Reaktor Innovations and University of Helsinki. -->

# Backing track generator

This project idea was crafted for the Building AI course final assignment.


## Summary

Backing track generator allows musicians to produce backing tracks from their favorite songs. Backing track generator takes a song in mp3 or wav format as input and generates a new version of the song without the sounds from selected instrument. With the help of backing track generator musicians can effectively practise songs or produce new arrangements (or solos!) for the songs.


## Background

Having an effective way to produce backing tracks has been a problem for aspiring musicians a long time. Musicians have tried to solve this problem previously by using tools such as [Guitar Pro](https://en.wikipedia.org/wiki/Guitar_Pro) or [Tuxguitar](https://en.wikipedia.org/wiki/TuxGuitar) which allow replicating existing songs by transcribing them and afterwards playback with selected instrument tracks and tempo. Since the original releases some software have evolved towards trying to use more realistic sound engines than the original MIDI sounds. This reflects that musicians desire to play along with as realistic sounds as possible. 

Wanting to play along with songs with realistic sounds has also spawned another way of coping with the problem: producing backing tracks using help of MIDI, VST instruments and DAWs. People producing these types of backing tracks have also uploaded them to video services such as Youtube. Usually the backing track is generated for practising with one type of instrument (such as guitar, bass or drums) but backing tracks consisting of only one instrument which allow practising with multiple different instruments do also exist.

Producing a backing track of a song is hard work and usually the quality does not match the quality of the original song. By utilizing neural networks to produce good quality backing tracks with desired instruments, musicians can finally focus the task they wish to focus: practising the songs they like (whether they enjoy huge popularity or not).


## How is it used?

The solution is an executable program downloadable and usable by musicians with their personal computers. Use of solution requires musicians to have a legal copy of the song they wish to transform in mp3 or wav file format. Since musicians may have any operating installed to their computer, the solution needs to support all most common operating systems (Windows, macOS, Linux). Support for as many different instruments as possible should be available in the solution so that musicians playing different instruments can utilize the solution. 


## Data sources and AI methods

The data needed to build the solution would require original multitrack files for a lot of songs so that a neural network could be trained using supervised learning paradigm. One way to use the data would be to use the final version of the song as input and use another version of the song which has some instrument's tracks disabled as target label. The type of neural network as well as the data format to be used would require research to be decided. 


## Challenges

Unability to access the required data is the reason why the solution cannot be implemented by any other than (probably) some large record label. Even in cases if the data was available, the project rises many copyright related questions that would need to be solved before implementing the proposed project.

In addition to the problem of gathering data and challenges with copyright, another problem that would need to be solved considers the format in which the data would need to be transformed before it could be used as input. One option for implementing the solution could be to use [spectrograms](https://en.wikipedia.org/wiki/Spectrogram) as the input format and convolutional neural networks for the method of constructing the neural network. However, since spectrogram is not a perfect way of describing sound it is possible that the method would result into a failure.


## What next?

This project, as it is currently defined, is not achievable because of the variety of challenges relating to the required data. Even if the problems with data acquisition were solved, a lot of research regarding audio processing for neural networks would need to be done. In addition, quite a lot help would be needed in generating the approariate dataset out of the raw data as every track would need to be exported multiple times. This would require a lot of both human resources as well as computational resources.
