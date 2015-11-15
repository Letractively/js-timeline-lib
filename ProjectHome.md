# JavaScript Timeline Library #

## Introduction ##

Draw a chart showing periods as a timeline in your browser using JavaScript.


## Usage ##

Insert this code in your page:

```

        <style type="text/css">
                .anoLine {
                        width: 2px;
                        background-color: #D8D8D8;
                }

                .anoText {
                        width: 365px;
                        display: inline-block;
                        left: -15px;
                        position: relative;
                }

                .anoContainer {
                        display: inline-block;
                }

                #mainCanvas {
                        position: relative;
                        overflow: auto;
                        white-space: nowrap;
                        background-color: #e5f7ca;
                        padding-left: 25px;
                }
        </style>

        <div id="mainCanvas">
             <!-- where timeline will be rendered -->
        </div>

        <script type="text/javascript" src="js-timeline-lib.js">
        </script>

        <script type="text/javascript">
                //date format: dd-mm-yyyy

                var periods = [
                                        ['20/03/1974', '15/09/1977'],
                                        ['06/03/1979', '28/02/1980'],
                                        ['01/12/1980', '17/06/1986'],
                                        ['23/06/1986', '17/10/2012'],
                                        ['13/01/1978', '07/12/1978'],
                                ];

                var timeline = new Timeline(periods);

                timeline.render();
        </script>
```

## Result ##

![http://js-timeline-lib.googlecode.com/files/screenshot-01.png](http://js-timeline-lib.googlecode.com/files/screenshot-01.png)