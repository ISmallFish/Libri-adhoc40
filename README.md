<img src="https://github.com/ISmallFish/Libri-adhoc40/blob/main/images/Libri-adhoc40.png" width="800">

# Libri-adhoc40
Libri-adhoc40 is a synchronized speech corpus, which collects the replayed Librispeech data from loudspeakers by ad-hoc microphone arrays of 40 strongly synchronized distributed nodes in a real office environment. Besides, to provide the evaluation target for speech frontend processing and other applications, it also recorded the replayed Librispeech data in an anechoic chamber.

## Description of the dataset
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

For each utterance in ‘train-clean-100’, ‘dev-clean’, and ‘test-clean’ corpora, we replayed it through loudspeaker both in the office room and the anechoic chamber. Besides, when we collected the training data in the office room, the positions of the microphones are different from those when collecting the development data and test data. 

### training data

#### Recording environment

##### room info

##### placements of microphones and loudspeakr

The plane structure of the office room is shown in Figure 1.

<img src="https://github.com/ISmallFish/Libri-adhoc40/blob/main/images/train_rec_pic.jpg" width="450">

### development and test data


## Download Link
The data can be downloaded at https://github.com/ISmallFish/Libri-adhoc40

## Reference
[Libri-adhoc40: A dataset collected from synchronized ad-hoc microphone arrays](https://arxiv.org/abs/2103.15118)

[Scaling sparsemax based channel selection for speech recognition with ad-hoc microphone arrays](https://arxiv.org/abs/2103.15305)
