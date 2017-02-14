<!DOCTYPE html>
<html lang="en">

<!-- Head tag -->
<head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="description" content="小车厂">
    <meta name="keyword" content="小车厂">
    <meta name="theme-color" content="#600090">
    <meta name="msapplication-navbutton-color" content="#600090">
    <meta name="apple-mobile-web-app-capable" content="yes">
    <meta name="apple-mobile-web-app-status-bar-style" content="#600090">
    <link rel="shortcut icon" href="https://cdn4.iconfinder.com/data/icons/ionicons/512/icon-person-128.png">
    <link rel="alternate" type="application/atom+xml" title="xiao" href="/atom.xml">
    <link rel="stylesheet" href="//cdnjs.cloudflare.com/ajax/libs/animate.css/3.5.2/animate.min.css">
    <link rel="stylesheet" href="//cdn.bootcss.com/font-awesome/4.6.3/css/font-awesome.css">
    <title>
        
        小车厂
        
    </title>

    <link rel="canonical" href="http://sunlianguang.github.io/">

    <!-- Bootstrap Core CSS -->
    <link rel="stylesheet" href="/css/bootstrap.min.css">

    <!-- Custom CSS -->
    <link rel="stylesheet" href="/css/blog-style.css">

    <!-- Pygments Github CSS -->
    <link rel="stylesheet" href="/css/syntax.css">
</head>

<style>
    @media all and (max-width: 768px) {
        header.intro-header {
            background-image: url('http://ohds8sy3t.bkt.clouddn.com/images/hexo/uteuunhvmls-engeland.jpg')
        }
    }
</style>
<!-- hack iOS CSS :active style -->
<body ontouchstart="" class="animated fadeIn">
<!-- Navigation -->
<nav class="navbar navbar-default navbar-custom navbar-fixed-top " id="nav-top" data-ispost = "false" data-istags="false
" data-ishome = "true" >
    <div class="container-fluid">
        <!-- Brand and toggle get grouped for better mobile display -->
        <div class="navbar-header page-scroll">
            <button type="button" class="navbar-toggle">
                <span class="sr-only">Toggle navigation</span>
                <span class="icon-bar"></span>
                <span class="icon-bar"></span>
                <span class="icon-bar"></span>
            </button>
            <a class="navbar-brand animated pulse" href="/">
                <span class="brand-logo">
                    xiao
                </span>
                's Blog
            </a>
        </div>

        <!-- Collect the nav links, forms, and other content for toggling -->
        <!-- Known Issue, found by Hux:
            <nav>'s height woule be hold on by its content.
            so, when navbar scale out, the <nav> will cover tags.
            also mask any touch event of tags, unfortunately.
        -->
        <!-- /.navbar-collapse -->
        <div id="huxblog_navbar">
            <div class="navbar-collapse">
                <ul class="nav navbar-nav navbar-right">
                    <li>
                        <a href="/">Home</a>
                    </li>
					
                    
                        
							
                        <li>
                            <a href="/Tags/">Tags</a>
                        </li>
							
						
                    
                        
							
						
                    
                        
							
                        <li>
                            <a href="/works/">works</a>
                        </li>
							
						
                    
					
					
                </ul>
            </div>
        </div>
    </div>
    <!-- /.container -->
</nav>
<script>
    // Drop Bootstarp low-performance Navbar
    // Use customize navbar with high-quality material design animation
    // in high-perf jank-free CSS3 implementation
//    var $body   = document.body;
    var $toggle = document.querySelector('.navbar-toggle');
    var $navbar = document.querySelector('#huxblog_navbar');
    var $collapse = document.querySelector('.navbar-collapse');

    $toggle.addEventListener('click', handleMagic)
    function handleMagic(e){
        if ($navbar.className.indexOf('in') > 0) {
        // CLOSE
            $navbar.className = " ";
            // wait until animation end.
            setTimeout(function(){
                // prevent frequently toggle
                if($navbar.className.indexOf('in') < 0) {
                    $collapse.style.height = "0px"
                }
            },400)
        }else{
        // OPEN
            $collapse.style.height = "auto"
            $navbar.className += " in";
        }
    }
</script>

<!-- Main Content -->


<style>

    .custom-haojen-container .post-preview:nth-of-type(1),
    .custom-haojen-container .post-preview-poetry:nth-of-type(1) {
        text-align: center;
        background-repeat: no-repeat;
        border-radius: 3px;
        background-size: cover;
        padding: 0;
        height: 300px;
        display: table;
        width: 100%;
        background-color: rgba(0, 0, 0, 0.16);
    }

    /*去掉诗歌的背景图片*/
    .custom-haojen-container .post-preview-poetry:nth-of-type(1) {
        background-image: none !important;
        background-color: rgba(255, 248, 220, 0.5);
    }

    .custom-haojen-container .post-preview:nth-child(1) h2,
    .custom-haojen-container .post-preview:nth-child(1) .post-meta,
    .custom-haojen-container .post-preview:nth-child(1) .post-subtitle {
        text-shadow: 0 0 40px rgba(0, 0, 0, 1);
        letter-spacing: 1px;
        color: #fff;
        margin-top: 0;
        padding-left: 60px;
        padding-right: 60px;
    }

    .custom-haojen-container .post-preview:nth-child(1) .post-meta {
        font-size: .9em;
        font-weight: 300;
        margin-top: 0;
    }

    .custom-haojen-container .post-preview-poetry:nth-child(1) .post-subtitle {
        letter-spacing: 6px;
        font-size: 18px;
        font-family: unset;
        font-weight: 400;
        color: rgba(0, 0, 0, .75)
    }

    /*不显示摘要*/
    .custom-haojen-container .post-preview:nth-child(1) .post-content-preview {
        display: none
    }

    /*只第一个显示背景图片*/
    .custom-haojen-container .post-preview:not(:nth-child(1)) {
        background-image: none !important;
    }

    /*第一个分界线去掉*/
    .custom-haojen-container hr:nth-of-type(1) {
        display: none;
    }

    /*主题*/
    .custom-haojen-container .post-preview:nth-of-type(1) > a {
        display: table-cell;
        vertical-align: middle;
    }

    /*诗词标题*/
    .custom-haojen-container .post-preview-poetry:nth-child(1) h2 {
        font-size: 35px;
        font-family: STKaiti;
        color: rgba(0, 0, 0, .8);
    }

    .custom-haojen-container .post-preview-poetry:nth-of-type(1) .post-meta {
        color: #0e2231;
    }

    @media (max-width: 768px) {
        .custom-haojen-container .post-preview:nth-child(1) {
            height: 240px;
        }

        .custom-haojen-container .post-preview-poetry:nth-child(1) h2 {
            font-size: 28px !important;
            margin-top: 0;
        }

        .custom-haojen-container .post-preview:nth-child(1) .post-subtitle {
            font-size: 18px;
            font-weight: 400;
            padding-left: 0;
            padding-right: 0;
        }

        .custom-haojen-container .post-preview:nth-of-type(1) > a {
            padding: 20px
        }
    }

    /*手机屏幕*/
    @media (max-width: 400px) {
        .custom-haojen-container .post-preview:nth-child(1) {
            height: 195px;
        }

        .custom-haojen-container .post-preview-poetry:nth-child(1) h2 {
            font-size: 20px !important;
        }

        .custom-haojen-container .post-preview:nth-child(1) .post-subtitle {
            font-size: 16px;
        }

        .custom-haojen-container .post-preview:nth-child(1) a {
            padding: 30px 20px;
        }
    }
</style>

<!-- Page Header -->
<div class="col-lg-8 col-lg-offset-2 col-md-10 col-md-offset-1 visible-xs-block visible-sm-block">
    <div class="row">
        <header class="intro-header">
            <div class="container">
                <div class="site-heading text-center">
                    <div class="about-me">
                        <!--移动端头部显示-->
                        <img src="http://ohds8sy3t.bkt.clouddn.com/images/hexo/sidebar_head.jpg"/>
                        <!--<h5><a href="/about/">小车厂</a></h5>-->
                        <!--修改-->
                        <h5><a href="/">小车厂</a></h5>
                        <p> </p>
                    </div>
                </div>
            </div>
        </header>
    </div>
</div>
<!-- Main Content -->
<div class="container custom-haojen-container">
    <!-- Post Container -->
    <div class="row">
        <div class="col-lg-8 col-lg-offset-1 col-md-8 col-md-offset-1 col-sm-12 col-xs-12 post-container">
            <!-- Main Content -->



<div class="post-preview "
     style="background-image: url('http://ohds8sy3t.bkt.clouddn.com/images/hexo/wallpaper (1).png')">
    <a href="/2016/11/29/Hello-My-World/">
        <h2 class="post-title">
            Welcome to My World
        </h2>
        <p class="post-meta">
            <i class="fa fa-calendar" aria-hidden="true"></i> 2016-11-29
        </p>
        
        <div class="post-content-preview">
            <p>
                
我的第一篇文章
在很久以前，就想用 Github Pages 建一个博客，于是就开始行动，当时选择的是 Github + Jkeyll ，昨天决定要重新做的时候也是用的 jekyll，但是遇到了很多无法解决的问题，比如说

在安装 Jekyll “gem install jekyll” 时报错..
            </p>
        </div>
    </a>

</div>

<hr>




<!-- 翻页 pager -->

<ul class="pager">
    
    
</ul>


        </div>
        <!-- Sidebar Container -->
        <div class="
                col-lg-3 col-lg-offset-0
                col-md-3 col-md-offset-0
                col-sm-12
                col-xs-12
                sidebar-container
            ">

            <!-- About Me -->
            <section class="visible-md visible-lg" style="padding: 0 18px">
                <div class="short-about">
                    <!--侧边栏头像-->
                    
                    <img src="http://ohds8sy3t.bkt.clouddn.com/images/hexo/sidebar_head.jpg"/>
                    
                    <!--<h5><a href="/about/">小车厂</a></h5>-->
                    <!--修改-->
                    <h5><a href="/">小车厂</a></h5>
                    
                    <p> </p>
                    
                    <hr>
                    <!-- SNS Link 社交 -->
                    <ul class="list-inline">
                        
                        
                        
                        <li>
                            <a target="_blank" href="https://www.zhihu.com/people/sunlg">
                                        <span class="fa-stack fa-lg">
                                            <i class="fa fa-circle fa-stack-2x"></i>
                                            <i class="fa  fa-stack-1x fa-inverse">知</i>
                                        </span>
                            </a>
                        </li>
                        

                        
                        <li>
                            <a target="_blank" href="http://weibo.com/xiaochechang">
                                        <span class="fa-stack fa-lg">
                                            <i class="fa fa-circle fa-stack-2x"></i>
                                            <i class="fa fa-weibo fa-stack-1x fa-inverse"></i>
                                        </span>
                            </a>
                        </li>
                        

                        

                        
                        <li>
                            <a target="_blank" href="https://github.com/sunlianguang">
                                        <span class="fa-stack fa-lg">
                                            <i class="fa fa-circle fa-stack-2x"></i>
                                            <i class="fa fa-github fa-stack-1x fa-inverse"></i>
                                        </span>
                            </a>
                        </li>
                        

                        
                    </ul>
                </div>
            </section>

            <!-- Featured Tags  标签 -->
            
            <section>
                <div class="tags">
                    
                    
                    
                    
                    
                </div>
            </section>
            

            
            <hr>
            <h5 style="text-align: center;">Friends</h5>
            <ul class="list-inline" style="text-align: center;">
                
                <li><a href="https://sunlianguang.github.io" target="_blank">小车厂（Github）</a></li>
                
                <li><a href="http://sunlianguang.coding.me" target="_blank">小车厂（Coding）</a></li>
                
            </ul>
            

        </div>
    </div>
</div>

<!-- Footer -->
<!-- Footer -->
<footer>
    <div class="container">
        <div class="row">
            <div class="col-lg-8 col-lg-offset-2 col-md-10 col-md-offset-1 text-center">
                <br>
<!--                 <ul class="list-inline text-center">
                
                
                
                    <li>
                        <a target="_blank" href="https://www.zhihu.com/people/sunlg">
                            <span class="fa-stack fa-lg">
                                <i class="fa fa-circle fa-stack-2x"></i>
                                <i class="fa  fa-stack-1x fa-inverse">知</i>
                            </span>
                        </a>
                    </li>
                

                
                    <li>
                        <a target="_blank" href="http://weibo.com/xiaochechang">
                            <span class="fa-stack fa-lg">
                                <i class="fa fa-circle fa-stack-2x"></i>
                                <i class="fa fa-weibo fa-stack-1x fa-inverse"></i>
                            </span>
                        </a>
                    </li>
                

                

                
                    <li>
                        <a target="_blank"  href="https://github.com/sunlianguang">
                            <span class="fa-stack fa-lg">
                                <i class="fa fa-circle fa-stack-2x"></i>
                                <i class="fa fa-github fa-stack-1x fa-inverse"></i>
                            </span>
                        </a>
                    </li>
                

                

                </ul> -->
                <p class="copyright text-muted">
                    Copyright &copy; xiao 2016
                    <br>
                    <span id="busuanzi_container_site_pv" style="font-size: 12px;">PV: <span id="busuanzi_value_site_pv"></span> Times</span>
                    <!--<br>-->
                    <!--Theme by <a href="https://haojen.github.io/">Haojen Ma</a>-->
                </p>

            </div>
        </div>
    </div>
</footer>

<!-- jQuery -->
<script src="/js/jquery.min.js"></script>

<!-- Bootstrap Core JavaScript -->
<script src="/js/bootstrap.min.js"></script>

<!-- Custom Theme JavaScript -->
<script src="/js/blog.js"></script>

<!--InstantClick 即时点击-->
<!--<script data-no-instant>-->
    <!--InstantClick.on('change', function(isInitialLoad) {-->
        <!--if (isInitialLoad === false) {-->
            <!--if (typeof MathJax !== 'undefined') // support MathJax-->
                <!--MathJax.Hub.Queue(["Typeset",MathJax.Hub]);-->
            <!--if (typeof prettyPrint !== 'undefined') // support google code prettify-->
                <!--prettyPrint();-->
            <!--if (typeof _hmt !== 'undefined')  // support 百度统计-->
                <!--_hmt.push(['_trackPageview', location.pathname + location.search]);-->
            <!--if (typeof ga !== 'undefined')  // support google analytics-->
                <!--ga('send', 'pageview', location.pathname + location.search);-->
        <!--}-->
    <!--});-->
    <!--InstantClick.init();-->
<!--</script>-->

<!-- async load function -->
<script>
    function async(u, c) {
      var d = document, t = 'script',
          o = d.createElement(t),
          s = d.getElementsByTagName(t)[0];
      o.src = u;
      if (c) { o.addEventListener('load', function (e) { c(null, e); }, false); }
      s.parentNode.insertBefore(o, s);
    }
</script>

<!-- jquery.tagcloud.js -->
<script>
    // only load tagcloud.js in tag.html
    if($('#tag_cloud').length !== 0){
        async("http://sunlianguang.github.io/js/jquery.tagcloud.js",function(){
            $.fn.tagcloud.defaults = {
                //size: {start: 1, end: 1, unit: 'em'},
                color: {start: '#bbbbee', end: '#0085a1'},
            };
            $('#tag_cloud a').tagcloud();
        })
    }
</script>

<!--fastClick.js -->
<script>
    async("//cdn.bootcss.com/fastclick/1.0.6/fastclick.min.js", function(){
        var $nav = document.querySelector("nav");
        if($nav) FastClick.attach($nav);
    })
</script>

<!-- Google Analytics -->



<!-- Baidu Tongji -->


<!-- swiftype -->
<script type="text/javascript">
  (function(w,d,t,u,n,s,e){w['SwiftypeObject']=n;w[n]=w[n]||function(){
  (w[n].q=w[n].q||[]).push(arguments);};s=d.createElement(t);
  e=d.getElementsByTagName(t)[0];s.async=1;s.src=u;e.parentNode.insertBefore(s,e);
  })(window,document,'script','//s.swiftypecdn.com/install/v2/st.js','_st');

  _st('install','null','2.0.0');
</script>

<script async src="//dn-lbstatics.qbox.me/busuanzi/2.3/busuanzi.pure.mini.js"></script>



<!--wechat title img-->
<img class="wechat-title-img" src="http://ohds8sy3t.bkt.clouddn.com/images/hexo/sidebar_head.jpg">
</body>

</html>
