# yii2-poll
Poll and google charts widget for yii2

The Poll and google charts widget for the Yii2 framework allows you to create custom polls and draw google charts for them .

<b>Installing</b>

The preferred way to install this extension is through composer.

Either run

    php composer.phar require "vkolya/poll-and-charts":"dev-master"
or add

    "vkolya/poll-and-charts":"dev-master"
to the require section of your application's composer.json file.

<b>Usage</b>

At first, import widget classes in view file where you want create poll

use vkolya\poll\myPoll; Then invoke the widget and specify the name of the poll and the response options

    echo myPoll::widget([
         'visualization' => 'PieChart',
         'pullName' => 'What framework do you know ?',
       
         'answerOptions'=>
                [
                 
            'Laravel',
            'Yii2',
            'Symfony',
                 
                ],
        'diagrammsOptions' => array(title => 'Frameworks',
            height => 300,
            width => 450,
                ),
                ])
<p align="center">
  <img src="https://github.com/Vkolya/poll-and-charts/blob/master/views/examp.jpg" width="350"/>
</p>
