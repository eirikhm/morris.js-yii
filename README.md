morris.js-yii
=============

[Morris.js](http://www.oesmith.co.uk/morris.js/) widget for [Yii Framework](http://www.yiiframework.com/)

Usage
=====

Place files in Yii's extension folder.

Chart Area
==
```php
$this->widget('application.extensions.morris.MorrisChartWidget', array(
    'id'      => 'myChartElement',
    'options' => array(
        'chartType' => MorrisChartWidget::CHART_AREA,
        'data'      => array(
            array('y' => 2006, 'a' => 100, 'b' => 90),
            array('y' => 2007, 'a' => 40, 'b' => 60),
            array('y' => 2008, 'a' => 50, 'b' => 10),
            array('y' => 2009, 'a' => 60, 'b' => 50),
            array('y' => 2010, 'a' => 60, 'b' => 40),
        ),
        'xkey'      => 'y',
        'ykeys'     => array('a', 'b'),
        'labels'    => array('Series A', 'Series B'),
    ),
));
```

Chart Line
==
```php
$this->widget('application.extensions.morris.MorrisChartWidget', array(
    'id'      => 'myChartElement',
    'options' => array(
        'chartType' => MorrisChartWidget::CHART_LINE,
        'data'      => array(
            array('y' => 2006, 'a' => 100, 'b' => 90),
            array('y' => 2007, 'a' => 40, 'b' => 60),
            array('y' => 2008, 'a' => 50, 'b' => 10),
            array('y' => 2009, 'a' => 60, 'b' => 50),
            array('y' => 2010, 'a' => 60, 'b' => 40),
        ),
        'xkey'      => 'y',
        'ykeys'     => array('a', 'b'),
        'labels'    => array('Series A', 'Series B'),
    ),
));
```

Chart Donut
==
```php
$this->widget('application.extensions.morris.MorrisChartWidget', array(
    'id'      => 'myChartElement',
    'options' => array(
        'chartType' => MorrisChartWidget::CHART_DONUT,
        'data'      => array(
            array('label' => 2006, 'value' => 12),
            array('label' => 2007, 'value' => 30),
            array('label' => 2008, 'value' => 20)
        ),
    ),
));
```


Chart Bar
==
```php
$this->widget('application.extensions.morris.MorrisChartWidget', array(
    'id'      => 'myChartElement',
    'options' => array(
        'chartType' => MorrisChartWidget::CHART_BAR,
        'data'      => array(
            array('y' => 2006, 'a' => 100, 'b' => 90),
            array('y' => 2007, 'a' => 40, 'b' => 60),
            array('y' => 2008, 'a' => 50, 'b' => 10),
            array('y' => 2009, 'a' => 60, 'b' => 50),
            array('y' => 2010, 'a' => 60, 'b' => 40),
        ),
        'xkey'      => 'y',
        'ykeys'     => array('a', 'b'),
        'labels'    => array('Series A', 'Series B'),
    ),
));
```




License
=======
BSD / MIT.