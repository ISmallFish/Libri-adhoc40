<img src="https://github.com/ISmallFish/Libri-adhoc40/blob/main/images/Libri-adhoc40.png" width="800">

# Libri-adhoc40
Libri-adhoc40 is a synchronized speech corpus, which collects the replayed Librispeech data from loudspeakers by ad-hoc microphone arrays of 40 strongly synchronized distributed nodes in a real office environment. Besides, to provide the evaluation target for speech frontend processing and other applications, it also recorded the replayed Librispeech data in an anechoic chamber.

## Description of the dataset
The Libri-adhoc40 dataset is built on the ‘train-clean-100’, ‘dev-clean’, and ‘test-clean’ corpora of Librispeech, which contains about 110 hours of US English speech from 331 speakers. Eventually, Libri-adhoc40 contains 4510 hours data in total with 110 hours data per microphone.

<table>
    <tr>
        <th>班级</th><th>课程</th><th>平均分</th>
    </tr>
    <tr>
        <td rowspan="3">1班</td><td>语文</td><td>95</td>
    </tr>
    <tr>
        <td>数学</td><td>96</td>
    </tr>
    <tr>
        <td>英语</td><td>92</td>
    </tr>
</table>

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-8fhc{font-family:"Trebuchet MS", Helvetica, sans-serif !important;;font-weight:bold;text-align:center;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-8fhc">subset</th>
    <th class="tg-8fhc">room info</th>
    <th class="tg-8fhc">total duration<br>（per channel）</th>
    <th class="tg-8fhc">spkr nums</th>
    <th class="tg-8fhc">ch nums</th>
    <th class="tg-8fhc">loudspeaker positions</th>
    <th class="tg-8fhc">playback corpus<br>in Librispeech</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-baqh">training data</td>
    <td class="tg-baqh" rowspan="3">office room<br></td>
    <td class="tg-baqh">100h</td>
    <td class="tg-baqh">251</td>
    <td class="tg-baqh">40</td>
    <td class="tg-baqh">9</td>
    <td class="tg-baqh">train-clean-100</td>
  </tr>
  <tr>
    <td class="tg-baqh">dev data</td>
    <td class="tg-baqh">5h</td>
    <td class="tg-baqh">40</td>
    <td class="tg-baqh">40</td>
    <td class="tg-baqh">4</td>
    <td class="tg-baqh">dev-clean</td>
  </tr>
  <tr>
    <td class="tg-baqh">test data</td>
    <td class="tg-baqh">5h</td>
    <td class="tg-baqh">40</td>
    <td class="tg-baqh">40</td>
    <td class="tg-baqh">4</td>
    <td class="tg-baqh">test-clean</td>
  </tr>
  <tr>
    <td class="tg-baqh">ground-truth clean data</td>
    <td class="tg-baqh">anechoic chamber</td>
    <td class="tg-baqh">110h</td>
    <td class="tg-baqh">331</td>
    <td class="tg-baqh">1</td>
    <td class="tg-baqh">1</td>
    <td class="tg-baqh">train-clean-100<br>dev-clean<br>test-clean</td>
  </tr>
</tbody>
</table>

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
