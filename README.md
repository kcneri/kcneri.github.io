# kcneri.github.io

<!DOCTYPE html>

<!--

                                  88         88
                                  88         ""
                                  88
        8b       d8  88       88  88   ,d8   88
        `8b     d8'  88       88  88 ,a8"    88
         `8b   d8'   88       88  8888[      88
          `8b,d8'    "8a,   ,a88  88`"Yba,   88
            Y88'      `"YbbdP'Y8  88   `Y8a  88
            d8'
           d8'     0.2.14

          Yuki by Cory Gibbons
          github.com/corygibbons/yuki

          hello@corygibbons.com
          corygibbons.com
          @corygibbons

-->

<html>
    <head>
        <title>{Title}</title>
        <link rel="shortcut icon" href="{Favicon}">
        <link rel="alternate" type="application/rss+xml" href="{RSS}">

        {block:Description}
          <meta name="description" content="{MetaDescription}" />
        {/block:Description}
        <meta name="viewport" content="width=device-width, initial-scale=1">

        <!-- jQuery -->
        <script src="http://static.tumblr.com/j9zrgpw/Pikmg130a/jquery-1.7.1.min.js"></script>

        <!-- Modernizr -->
        <script src="http://static.tumblr.com/j9zrgpw/3iymg1311/modernizr-1.7.min.js"></script>

        <!--[if IE]>
            <script src="http://static.tumblr.com/j9zrgpw/Sa4n3cja6/html5.js"></script>
        <![endif]-->

        <!-- Stylesheet -->
        <link rel="stylesheet" type="text/css" href="http://static.tumblr.com/j9zrgpw/MFon38qg7/style.css"/>
        <link rel="stylesheet" type="text/css" href="http://static.tumblr.com/j9zrgpw/ZyFn3civd/font-awesome.css">

        <!-- Defaults -->
        <meta name="color:Post Hover" content="#fbfbfb"/>
        <meta name="select:Scroll" content="click" title="Click to Load">
        <meta name="select:Scroll" content="automatic" title="Automatic">
        <meta name="if:Infinite Scroll" content="1"/>
        <meta name="if:Notes" content="0"/>
        <meta name="if:Show Full Photoset" content="0">

        <style type="text/css">
        .post-background { background: {color:Post Hover}; }
        {block:IndexPage} {block:IfNotShowFullPhotoset}.post .photoset { display: none; } .post .photoset:first-child { display: block; }{/block:IfNotShowFullPhotoset}{/block:IndexPage}
        {CustomCSS}
        </style>

    </head>

<body>

<div id="container">

    <header class="main">

        <div class="title fade">
            <h1><a href="/">{Title}</a></h1>
            {block:HasPages}
                /
                {block:Pages}
                    <span class="page"><a href="{URL}">{Label}</a></span>
                {/block:Pages}
            {/block:HasPages}
        </div>


        {block:TagPage}
            <div class="tagged fade">
                Viewing all entries marked "{Tag}"
            </div>
        {/block:TagPage}

    </header>






    <section id="posts">

    {block:Posts}

        {block:Post1}
            {block:IndexPage}
                <section class="post fade double">
            {/block:IndexPage}

            {block:PermalinkPage}
                <section class="post fade double">
            {/block:PermalinkPage}
        {/block:Post1}



        {block:Post2}</section><section class="post fade single">{/block:Post2}
        {block:Post3}</section><section class="post fade single">{/block:Post3}
        {block:Post4}</section><section class="post fade single">{/block:Post4}
        {block:Post5}</section><section class="post fade single">{/block:Post5}
        {block:Post6}</section><section class="post fade double">{/block:Post6}
        {block:Post7}</section><section class="post fade single">{/block:Post7}
        {block:Post8}</section><section class="post fade single">{/block:Post8}
        {block:Post9}</section><section class="post fade single">{/block:Post9}
        {block:Post10}</section><section class="post fade single">{/block:Post10}
        {block:Post11}</section><section class="post fade double">{/block:Post11}
        {block:Post12}</section><section class="post fade single">{/block:Post12}
        {block:Post13}</section><section class="post fade single">{/block:Post13}
        {block:Post14}</section><section class="post fade single">{/block:Post14}
        {block:Post15}</section><section class="post fade single">{/block:Post15}





        {block:Text}
        <!-- Text Post -->
            <div class="text">

                {Block:PermalinkPage}
                    <hr>
                {/Block:PermalinkPage}

                {block:Title}
                    <h2><a href="{Permalink}">{Title}</a></h2>
                {/block:Title}

                <div class="text-body">
                    {Body}
                </div>

            </div>
        {/block:Text}





        {block:Photo}
        <!-- Photo post -->

            {block:IndexPage}
                <div class="post-background">
                    <a href="{Permalink}"><img src="{PhotoURL-HighRes}" alt="{PhotoAlt}"/></a>
                </div>
            {/block:IndexPage}

            {block:PermalinkPage}
                <div class="post-background">
                    <img src="{PhotoURL-HighRes}" alt="{PhotoAlt}"/>
                </div>
                {block:Caption}
                    <div class="caption">{Caption}</div>
                {/block:Caption}
            {/block:PermalinkPage}

        {/block:Photo}





        {block:Photoset}
        <!-- Photoset post -->

            {block:Photos}

                {Block:IndexPage}
                    <div class="photoset post-background">
                        <a href="{Permalink}"><img src="{PhotoURL-500}" width="{PhotoWidth-500}"height="{PhotoHeight-500}" /></a>
                    </div>
                {/Block:IndexPage}

                {Block:PermalinkPage}
                    <div class="photoset post-background">
                        <img src="{PhotoURL-HighRes}" width="{PhotoWidth-HighRes}"height="{PhotoHeight-HighRes}" />
                    </div>
                {/Block:PermalinkPage}

            {/block:Photos}

            {Block:PermalinkPage}
                {block:Caption}
                    <div class="caption">{Caption}</div>
                {/block:Caption}
            {/Block:PermalinkPage}

        {/block:Photoset}





        {block:Video}
        <!-- Video post -->

            {Block:IndexPage}
                <div class="video post-background">
                    {block:VideoThumbnail}
                        <a href="{Permalink}">
                            <img src="{VideoThumbnailURL}" />
                            <div class="video-play-button"></div>
                        </a>
                    {/block:VideoThumbnail}
                </div>
            {/Block:IndexPage}

            {Block:PermalinkPage}
                <div class="video post-background">
                    {Video-700}
                </div>

                {block:Caption}
                    <div class="caption">{Caption}</div>
                {/block:Caption}
            {/Block:PermalinkPage}

        {/block:Video}



        {block:Audio}
        <!-- Audio post -->
            <div class="audio">

                {Block:IndexPage}
                    {block:AudioEmbed}
                        {AudioEmbed-640}
                    {/block:AudioEmbed}
                {/Block:IndexPage}

            </div>
        {/block:Audio}





        {block:Quote}
        <!-- Quote post -->

            <div class="quote">
                "{Quote}"

                {block:Source}
                    <div class="source">{Source}</div>
                {/block:Source}
            </div>

        {/block:Quote}





        {block:Chat}
        <!-- Chat post -->

            <div class="chat">

                {block:Title}
                    <h3><a href="{Permalink}">{Title}</a></h3>
                {/block:Title}

                <ul class="chat">
                    {block:Lines}
                        <li class="{Alt} user_{UserNumber}">
                            {block:Label}
                                <span class="label">{Label}</span>

                            {/block:Label}

                            {Line}
                        </li>
                    {/block:Lines}
                </ul>

            </div>

        {/block:Chat}





        {block:Link}
        <!-- Link post -->

            <div class="link">
                <a href="{URL}" class="link-title" {Target}>{Name} <i class="fa fa-external-link fa-fw"></i></a>

                {block:Description}
                    <div class="description">{Description}</div>
                {/block:Description}
            </div>

        {/block:Link}





        {block:PermalinkPage}
            </section> <!-- img section -->

            {block:Date}
                <section class="post fade single navigation">
                    <header>Posted</header>
                    {Month} {DayOfMonth}, {Year}
                </section>
            {/block:Date}


            {block:HasTags}
                <section class="post fade single navigation">
                    <header>{lang:Tagged}</header>
                    {block:Tags}
                        <a href="{TagURL}">{Tag}</a>&nbsp;
                    {/block:Tags}
                </section>
            {/block:HasTags}


            {block:ContentSource}
                <section class="post fade single navigation">
                    <header>{lang:Source}</header>
                    <a href="{SourceURL}" target="_blank">{SourceTitle}</a>
                </section>
            {/block:ContentSource}


            {block:RebloggedFrom}
                <section class="post fade single navigation">
                    <header>{lang:Reblogged from}</header>
                    <a href="{ReblogParentURL}" target="_blank">{ReblogParentTitle}</a>
                </section>
            {/block:RebloggedFrom}


            {block:IfNotes}
                {block:PostNotes}
                    <section class="post fade notes-container testclass">
                        {block:NoteCount}
                            <header>{NoteCountWithLabel}</header>
                        {/block:NoteCount}
                        {PostNotes}
                    </section>
                {/block:PostNotes}
            {/block:IfNotes}



        {/block:PermalinkPage}



    {/block:Posts}

    {block:IndexPage}</section>{/block:IndexPage}

    </section>



    {block:Pagination}

        {block:PreviousPage}
            <section class="navigation">
                <a href="{PreviousPage}">{lang:Previous page}</a>
            </section>
        {/block:PreviousPage}

        {block:NextPage}
            <section class="navigation">
                <a href="{NextPage}" class="next-page">{lang:Next page}</a>
            </section>
        {/block:NextPage}

    {/block:Pagination}


</div> <!-- #container -->

{block:IndexPage}
    <footer class="primary-footer fade">
        <a href="#" class="load-more"><span class="load-more-entries">+</span></a>
    </footer>
{/block:IndexPage}


<script src="http://static.tumblr.com/iwtk77u/Yhym2yygt/jquery.imagesloaded.min.js"></script>
<!-- jQuery Masonry -->
<script src="http://static.tumblr.com/j9zrgpw/M6qmg12yb/jquery.masonry.min.js"></script>
<script src="http://static.tumblr.com/wgijwsy/u2vm2hxv6/jquery.infinitescroll.min.js"></script>

<script>
(function () {

    function resizeVideo(){
        var $video = $('.tumblr_video_container');

        var videoWidth = $video.width(),
            videoHeight = $video.height(),
            videoRatio = (videoHeight/videoWidth),

            newWidth = 560,
            newHeight = Math.floor(newWidth*videoRatio),

            mobileWidth = 260,
            mobileHeight = Math.floor(mobileWidth*videoRatio);

        if ($(window).width() < 640) {
            $video.css('width', '100%').css('height', mobileHeight);
            $video.find('iframe').height(mobileHeight);
        }
        else {
            $video.css('width', '100%').css('height', newHeight);
            $video.find('iframe').height(newHeight);
        }

        $(window).resize(function() {
            if ($(window).width() < 640) {
                $video.css('width', '100%').css('height', mobileHeight);
            }
            else {
                $video.css('width', '100%').css('height', newHeight);
            }
        });
    }
    resizeVideo();

    var $load_style = "{select:Scroll}";
    var $tumblelog = $('#posts');

    {block:IfInfiniteScroll}
        var $fade = $('.fade');
    {/block:IfInfiniteScroll}
    {block:IfNotInfiniteScroll}
        var $fade = $('.fade, .navigation, .notes');
    {/block:IfNotInfiniteScroll}

    $tumblelog.infinitescroll(
        {block:IfInfiniteScroll}
            {
            debug: true,
            loading: {
                img: 'data:image/gif;base64,R0lGODlhAQABAHAAACH5BAUAAAAALAAAAAABAAEAAAICRAEAOw==',
                finished: undefined,
                finishedMsg: '',
                msg: null,
                msgText: '',
                speed: 'fast',
                start: undefined
            },
            state: {
                currPage: {CurrentPage}
            },
            navSelector: ".navigation",
            nextSelector: ".navigation a.next-page",
            itemSelector: ".post",
            errorCallback: function (selector, msg) {
                $('.load-more').animate({
                    opacity: 0
                });
            }
        },
    {/block:IfInfiniteScroll}

    function (newElements) {
        var $newElems = $(newElements).css({
            opacity: 0
        });
        $newElems.imagesLoaded(function () {
            $newElems.animate({
                opacity: 1
            }).fadeIn();

            $tumblelog.masonry('appended', $newElems);

            $(".post").hover(function() {
                $(this).find('img').stop().animate({"opacity": "0.4"}, 300);
            }, function() {
                $(this).find('img').stop().animate({"opacity": "1"}, 300);
            });

        });
    });
    $tumblelog.imagesLoaded(function () {
        $fade.each(function(i) {
            $(this).delay(110*i).fadeIn();
        });

        $tumblelog.masonry({
            columnWidth: 300,
            isFitWidth: true,
            isAnimated: !Modernizr.csstransitions
        });
    });

    if ($load_style == "click" ) {
        $(window).unbind('.infscr');
        $( ".load-more" ).click(function() {
            $('#posts').infinitescroll('retrieve');
            return false;
        });
    }
    else {
        $('.load-more').remove();
    }

    {block:IfNotInfiniteScroll}
        $('.load-more').remove();
    {/block:IfNotInfiniteScroll}

})();
</script>

    </body>
</html>
