# BLOGPAGE
*{
    --main-color: #d3ad7f;
    --black: #13131a;
    --bg: #010103;
    --border: .1rem solid rgba(255, 255, 255, .3);
}

* {
    font-family: 'Roboto', sans-serif;
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    outline: none;
    border: none;
    text-decoration: none;
    text-transform: capitalize;
    transition: .2s linear;
}

html {
    font-size: 62.5%;
    overflow-x: hidden;
    scroll-padding-top: 9rem;
    scroll-behavior: smooth;
}

img {
    margin-left: 40px;
    border-radius: 50%;

}

h3 {
    color: black;
}
#home {
    background: url(https://r4.wallpaperflare.com/wallpaper/910/1001/198/sky-mountain-nature-ridge-wallpaper-d8560da840e0fc08504c210ec8c2640a.jpg);
    background-repeat: no-repeat;
    background-size: 1500px 700px;
}
/*width*/

html::-webkit-scrollbar {
    width: .8rem;
}

html::-webkit-scrollbar-track {
    background: transparent;
}

html::-webkit-scrollbar-thumb {
    background: #fff;
    border-radius: .5rem;
}

body {
    background: var(--black);
}

section {
    padding: 2rem 7%;
}

.heading {
    text-align: center;
    color: black;
    text-transform: uppercase;
    padding-bottom: 3.5rem;
    font-size: 4rem;
}

.heading span {
    color: var(--main-color);
    text-transform: uppercase;
}

.btn {
    margin-top: 1rem;
    display: inline-block;
    padding: .9rem 3rem;
    font-size: 1.7rem;
    color: #fff;
    background: var(--main-color);
    cursor: pointer;
}

.btn:hover {
    letter-spacing: .2rem;
}

.header {
    background: var(--black);
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 1.5rem 7%;
    border-bottom: var(--border);
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    z-index: 1000;
}

.header.logo img {
    height: 6rem;
}

.header .navbar a {
    margin: 0 1rem;
    font-size: 2rem;
    color: white;
}

.header .navbar a:hover {
    color: var(--main-color);
    border-bottom: .1rem solid var(--main-color);
    padding-bottom: .5rem;
}

.header .icons div {
    color: #fff;
    cursor: pointer;
    font-size: 2.5rem;
    margin-left: .9rem;
}

.header .icons div:hover {
    color: var(--main-color);
}

#menu-btn {
    display: inline-block;
}

.header .search-form {
    position: absolute;
    top: 115%;
    right: 7%;
    background: #fff;
    width: 50rem;
    height: 5rem;
    display: flex;
    align-items: center;
    transform: scaleY(0);
    transform-origin: top;
}

.header .search-form input {
    height: 100%;
    width: 100%;
    font-size: 1.6rem;
    color: var(--black);
    padding: 1rem;
    text-transform: none;
}

.header .search-form label {
    cursor: pointer;
    font-size: 2.2rem;
    margin-right: 1.5rem;
    color: var(--black);
}

.header .search-form label:hover {
    color: var(--main-color);
}

.header .cart-items-container {
    position: absolute;
    top: 100%;
    right: -100%;
    /* checkout list hide =o%*/
    height: calc(100vh - 9.5rem);
    width: 35rem;
    background: #fff;
    padding: 0 1.5rem;
}

.header .cart-items-container .cart-item {
    position: relative;
    margin: 2rem 0;
    display: flex;
    align-items: center;
    gap: 1.5rem;
}

.header .cart-items-container .cart-item .fa-times {
    position: absolute;
    top: 1rem;
    right: 1rem;
    font-size: 2rem;
    cursor: pointer;
    color: var(--black)/* cross sign */
}

.header .cart-items-container .cart-item .fa-times:hover {
    color: var(--main-color);
}

.header .cart-items-container .cart-item img {
    height: 8rem;
}

.header .cart-items-container .cart-item .content h3 {
    font-size: 2rem;
    color: var(--black);
    padding-bottom: .5rem;
}

.header .cart-items-container .cart-item .content .price {
    font-size: 1.5rem;
    color: var(--main-color);
}

.header .cart-items-container .btn {
    width: 100%;
    text-align: center;
}


/* media queries */

@media (max-width:991px) {
    html {
        font-size: 55%;
    }
    .header {
        padding: 1.5rem 2rem;
    }
    section {
        padding: 2rem;
    }
}

@media (max-width:768px) {
    #menu-btn {
        display: inline-block;
    }
    .header .navbar {
        position: absolute;
        top: 100%;
        right: -100%;
        background: #fff;
        width: 30rem;
        height: calc(100vh - 9.5vh);
    }
    .header .navbar a {
        color: var(--black);
        display: block;
        margin: 1.5rem;
        padding: .5rem;
        font-size: 2rem;
    }
    .home {
        background-position: left;
        justify-content: center;
        text-align: center;
    }
    .home.content h3 {
        font-size: 4.5rem;
    }
    .home.content p {
        font-size: 1.5rem;
    }
}

@media (max-width:450px) {
    html {
        font-size: 50%;
    }
}

.home {
    min-height: 100vh;
    display: flex;
    align-items: center;
    background-image: url(michal-parzuchowski-ItaV89TNkks-unsplash.jpg);
    background-size: cover;
    background-position: center;
}

.home .content {
    max-width: 60rem;
}

.home .content h3 {
    font-size: 6rem;
    text-transform: uppercase;
    color: #fff;
}

.home .content p {
    font-size: 2rem;
    font-weight: lighter;
    line-height: 1.8;
    padding: 1rem 0;
    color: #eee;
}

.about .row {
    /*bgc color */
    display: flex;
    align-items: center;
    background: var(--black);
    flex-wrap: wrap;
}

.about .row .image {
    flex: 1 1 45rem;
}

.about .row .image img {
    width: 90%;
}

.about .row .content {
    flex: 1 1 45rem;
    padding: 2rem;
}

.about .row .content h3 {
    font-size: 3rem;
    color: #fff;
}

.about .row .content p {
    font-size: 1.6rem;
    color: #ccc;
    padding: 1rem 0;
    line-height: 1.8;
}


/* review section */

.review .box-container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(30rem, 1fr));
    gap: 1.5rem;
}

.review .box-container .box {
    border: var(--border);
    text-align: center;
    padding: 3rem 2rem;
}

.review .box-container .box p {
    font-size: 1.5rem;
    line-height: 1.8;
    color: #fff;
    padding: 2rem 0;
}

.review .box-container .box .user {
    height: 13rem;
    width: 13rem;
    object-fit: cover;
    align-items: center;
}

.review .box-container .box h3 {
    padding: 1rem 0;
    font-size: 2rem;
    color: #fff;
}

.review .box-container .box .stars i {
    font-size: 1.5rem;
    color: var(--main-color);
}


/* contact section */

.contact .row {
    display: flex;
    background: var(--black);
    flex-wrap: wrap;
    gap: 1rem;
}

.contact .row .map {
    flex: 1 1 45rem;
    width: 100%;
    object-fit: cover;
}

.contact .row form {
    flex: 1 1 45rem;
    padding: 5rem 2rem;
    text-align: center;
}

.contact .row form h3 {
    text-transform: uppercase;
    font-size: 3.5rem;
    color: #fff;
}

.contact .row form .inputbox {
    display: flex;
    align-items: center;
    margin-top: 2rem;
    margin-bottom: 2rem;
    background: var(--bg);
    border: var(--border);
}

.contact .row form .inputbox span {
    color: #fff;
    font-size: 2rem;
    padding-left: 2rem;
}

.contact .row form .inputbox input {
    width: 100%;
    padding: 2rem;
    font-size: 1.7rem;
    color: #fff;
    text-transform: none;
    background: none;
}

.blogs .box-container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(30rem, 1fr));
    gap: 1.5rem;
}

.blogs .box-container .box {
    border: var(--border);
}

.blogs .box-container .box .image {
    height: 25rem;
    overflow: hidden;
    width: 100%;
}

.blogs .box-container .box .image img {
    height: 20rem;
    object-fit: cover;
    width: 90%;
    margin-right: 40rem;
}

.blogs .box-container .box:hover .image img {
    transform: scale(1.1);
}

.blogs .box-container .box .content {
    padding: 2rem;
}

.blogs .box-container .box .content .title {
    font-size: 2.5rem;
    line-height: 1.5rem;
    color: #fff;
}

.blogs .box-container .box .content .title:hover {
    color: var(--main-color);
}

.blogs .box-container .box .content span {
    color: var(--main-color);
    display: block;
    padding-top: 1rem;
    font-size: 2rem;
}

.blogs .box-container .box .content p {
    font-size: 1.6rem;
    line-height: 1.8;
    color: #ccc;
    padding: 1rem 0;
}


/* footer section */

.footer {
    background: var(--black);
    text-align: center;
}

.footer .share {
    padding: 1rem 0;
}

.footer .share a {
    height: 5rem;
    width: 5rem;
    line-height: 5rem;
    font-size: 2rem;
    color: #fff;
    border: var(--border);
    margin: .3rem;
    border-radius: 50%;
}

.footer .share a:hover {
    background-color: var(--main-color);
}

.footer .links {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    padding: 2.1rem 0;
    gap: 1rem;
}

.footer .links a {
    padding: .7rem 2rem;
    color: #fff;
    border: var(--border);
    font-size: 2rem;
}

.footer .links a:hover {
    background: var(--main-color);
}

.footer .credit {
    font-size: 2rem;
    color: #fff;
    font-weight: lighter;
    padding: 1.5rem;
}

.footer .credit span {
    color: var(--main-color);
}
