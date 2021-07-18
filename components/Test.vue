<template lang="pug">
    div
        div(class='nav')
            ul(class="navbar")
                li(class="icon")
                    a(href="#")
                        img(src="images/hambergur.png" class="icon-size hamburger-icon")
                    a(href="#")
                        img(src="images/logo.jpg" class="logo")
                li(class="search") 
                    input(type="serch" placeholder="搜尋" class="search-input")
                    button(class="search-btn") GO
                li 
                    a(href="#")
                        img(src="images/video-camera.png" class="icon-size rwd-icon")
                    a(href="#")
                        img(src="images/menu.png" class="icon-size rwd-icon")
                    a(href="#")
                        img(src="images/bell.png" class="icon-size rwd-icon")
                    a(href="#")
                        img(src="images/search.png" class="search-icon")
                    a(href="#")
                        img(src="https://yt3.ggpht.com/ytc/AKedOLT2yFgGvdTfRki_5DjuxDIg6ZnspFftDNcM-RGeYA=s88-c-k-c0x00ffffff-no-rj" class="icon-size personal-icon")
        div(class="tag") 
            button(class="category active") All
            button(v-for="i in 20" :key="i" class="category") tag {{ i }}
        div(class="main")
            ul(class="sidebar-container")
                li(v-for="i in 20" :key="i" class="sidebar-container-content")
                    a(href="#") sidebarContent
            div(class="content")
                div(class="cards" v-for="i in 30" :key="i")
                    a(href="#" data-time="2:30" class="video-img")
                        img(src="https://i.ytimg.com/vi/B1tArM5XYuc/hq720.jpg?sqp=-oaymwEcCNAFEJQDSFXyq4qpAw4IARUAAIhCGAFwAcABBg==&rs=AOn4CLBuGsK_uMdikkLprW8goa2KawvnEg" class="cover")
                    div(class="video-detail")
                        a(href="#")
                            img(src="https://yt3.ggpht.com/ytc/AKedOLT2yFgGvdTfRki_5DjuxDIg6ZnspFftDNcM-RGeYA=s88-c-k-c0x00ffffff-no-rj" class="channel-logo")
                        div(class="video-text")
                            a(href="#" class="video-title") 
                                    | 熊仔 Kumachan - 
                                    br
                                    | [88BARS] official Music...
                            a(href="#" class="video-content") 熊仔
                            p(class="video-content") 觀看次數 : 230萬次 ．
                            p(class="video-content") 4個月前
        div(class="footer")
            ul(class="footer-icon")
                li(class="footer-content")
                    img(src="images/house-black-silhouette-without-door.png" class="icon-size del-margin")
                    p 首頁
                li(class="footer-content")
                    img(src="images/trending.png" class="icon-size del-margin")
                    p 熱門
                li(class="footer-content")
                    img(src="images/subscript.png" class="icon-size del-margin")
                    p 訂閱
                li(class="footer-content")
                    img(src="images/book.png" class="icon-size del-margin")
                    p Library
</template>
