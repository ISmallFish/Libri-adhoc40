<img src="https://github.com/ISmallFish/Libri-adhoc40/blob/main/images/Libri-adhoc40.png" width="800">

# **Libri-adhoc40**
  Libri-adhoc40 is a synchronized speech corpus, which collects the replayed Librispeech data from loudspeakers by ad-hoc microphone arrays of 40 strongly synchronized distributed nodes in a real office environment. Besides, to provide the evaluation target for speech frontend processing and other applications, it also recorded the replayed Librispeech data in an anechoic chamber.

## **Description of the dataset**
  The Libri-adhoc40 dataset is built on the ‘train-clean-100’, ‘dev-clean’, and ‘test-clean’ corpora of Librispeech, which contains about 110 hours of US English speech from 331 speakers. Eventually, Libri-adhoc40 contains 4510 hours data in total with 110 hours data per microphone.

> an overview of **Libri-adhoc40** is listed in the following table:
> 
<table>
<thead>
  <tr>
    <th>subset</th>
    <th>recording<br>environment</th>
    <th>duration<br>per channel</th>
    <th>spkr nums</th>
    <th>ch nums</th>
    <th>loudspeaker positions</th>
    <th>playback corpus<br>in Librispeech</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>training data</td>
    <td rowspan="3">office room<br></td>
    <td>100h</td>
    <td>251</td>
    <td>40</td>
    <td>9</td>
    <td>train-clean-100</td>
  </tr>
  <tr>
    <td>dev data</td>
    <td>5h</td>
    <td>40</td>
    <td>40</td>
    <td>4</td>
    <td>dev-clean</td>
  </tr>
  <tr>
    <td>test data</td>
    <td>5h</td>
    <td>40</td>
    <td>40</td>
    <td>4</td>
    <td>test-clean</td>
  </tr>
  <tr>
    <td>ground-truth clean data</td>
    <td>anechoic chamber</td>
    <td>110h</td>
    <td>331</td>
    <td>1</td>
    <td>1</td>
    <td>train-clean-100<br>dev-clean<br>test-clean</td>
  </tr>
</tbody>
</table>

  For each utterance in ‘train-clean-100’, ‘dev-clean’, and ‘test-clean’ corpora, we replayed it through loudspeaker both in the office room and the anechoic chamber. Besides, when we collected the training data in the office room, the positions of the 40 microphones are different from those when collecting the development data and test data. 

  Assume that the sentence with the number of '229-130880-0017' was replayed, where number '229-130880-0017' means that speaker '229' speaked according to sentence '0017' in chapter '130880'. The naming rule can be described as follows:
> We can obtained 41 channels of data in total, since we recorded it in the office room and the anechoic chamber respectively. For each sentence we recorded, we first classified them according to the position of loudspeaker and speaker, then according to the chapters, and finally according to the orginal sentences number. Specifically, for each utterance recorded in the office room, we created a new name for it through adding a suffix to the original number ('174-84280-0010') according to the number of the microphone. As for the utterances recorded in anechoic chamber, a suffix named 'anechoic' is added at the end of each utterance.
>> In Librispeech corpus, the relative path of sentence '229-130880-0017' is:
>> ```
>> .\train-clean-100\229\130880\229-130880-0017.flac
>> ```
>> 
>> In Libri-adhoc40 corpus, the relative path of recorded sentences from '229-130880-0017' have the following forms: 
>> ```
>> .\adhoc40-train\pos #\229\130880\229-130880-0017-ch-1.wav
>> .\adhoc40-train\pos #\229\130880\229-130880-0017-ch-2.wav
>> .\adhoc40-train\pos #\229\130880\229-130880-0017-ch-3.wav
>>                          ...
>> .\adhoc40-train\pos #\229\130880\229-130880-0017-ch-40.wav
>> .\adhoc40-train\pos #\229\130880\229-130880-0017-anechoic.wav
>> ```
>> The `pos #` indicates the position of loudspeaker. See below for more detailed descriptions.

### **Training data**

#### **Recording environment**

The plane structure of the office room are as shown below. The red dot indicates the origin of the reference axes. The blue dots indicate the positions of the microphones, whose coordinates are listed in the upper-left corner. The positions and orientations of the loudspeaker are marked by loudspeaker icons. The terms ‘pos’ is short for position. The term ‘mic’ is short for microphone

<img src="https://github.com/ISmallFish/Libri-adhoc40/blob/main/images/train_rec_pic.jpg" width="450">



### development and test data


## Download Link
The data can be downloaded at https://github.com/ISmallFish/Libri-adhoc40

## Reference
[Libri-adhoc40: A dataset collected from synchronized ad-hoc microphone arrays](https://arxiv.org/abs/2103.15118)

[Scaling sparsemax based channel selection for speech recognition with ad-hoc microphone arrays](https://arxiv.org/abs/2103.15305)
