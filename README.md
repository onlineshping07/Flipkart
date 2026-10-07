# Flipkart<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Flipkárt - Online Shopping</title>

<meta name="description"
content="Flipkárt - Shop mobiles, electronics, fashion, home, beauty and more.">

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial,Helvetica,sans-serif;
}

body{
    background:#f1f3f6;
    color:#212121;
}

button{
    cursor:pointer;
    border:0;
}

a{
    text-decoration:none;
    color:inherit;
}

/* ================= HEADER ================= */

header{
    background:#2874f0;
    color:white;
    padding:10px 5%;
    display:flex;
    align-items:center;
    gap:20px;
    position:sticky;
    top:0;
    z-index:1000;
}

.logo{
    width:140px;
}

.logo h1{
    font-size:27px;
    font-style:italic;
}

.logo p{
    font-size:11px;
    color:#fff;
}

.logo span{
    color:#ffe500;
    font-weight:bold;
}

.search{
    flex:1;
    display:flex;
    max-width:700px;
}

.search input{
    width:100%;
    padding:13px 16px;
    border:0;
    outline:none;
    font-size:15px;
}

.search button{
    width:55px;
    background:white;
    color:#2874f0;
    font-size:20px;
}

.login{
    background:white;
    color:#2874f0;
    padding:10px 25px;
    font-weight:bold;
}

.header-link{
    font-weight:bold;
    white-space:nowrap;
}

/* ================= CATEGORY ================= */

.categories{
    background:white;
    display:flex;
    justify-content:center;
    gap:35px;
    padding:14px;
    overflow-x:auto;
    box-shadow:0 1px 4px #ddd;
}

.category{
    min-width:75px;
    text-align:center;
    font-weight:bold;
    font-size:13px;
}

.category-icon{
    font-size:30px;
    margin-bottom:6px;
}

/* ================= HERO ================= */

.hero{
    max-width:1450px;
    height:330px;
    margin:15px auto;
    background:linear-gradient(100deg,#2874f0,#00a8ff);
    color:white;
    display:flex;
    align-items:center;
    justify-content:space-between;
    padding:45px 9%;
    overflow:hidden;
}

.hero-content h1{
    font-size:46px;
    margin-bottom:12px;
}

.hero-content h2{
    font-size:25px;
    margin-bottom:15px;
}

.hero-content p{
    font-size:18px;
    margin-bottom:25px;
}

.hero-btn{
    background:#ff9f00;
    color:white;
    padding:14px 30px;
    font-weight:bold;
    font-size:15px;
}

.hero-art{
    font-size:180px;
}

/* ================= MAIN ================= */

.container{
    max-width:1450px;
    margin:auto;
}

.section{
    background:white;
    margin:15px 0;
    padding:22px;
}

.section-header{
    display:flex;
    align-items:center;
    justify-content:space-between;
    border-bottom:1px solid #eee;
    padding-bottom:15px;
    margin-bottom:20px;
}

.section-header h2{
    font-size:24px;
}

.view{
    background:#2874f0;
    color:white;
    padding:10px 20px;
    font-weight:bold;
}

/* ================= DEAL CARDS ================= */

.deals{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:18px;
}

.deal{
    min-height:180px;
    padding:25px;
    border-radius:5px;
    background:#f8f9fa;
    text-align:center;
}

.deal-icon{
    font-size:60px;
    margin-bottom:12px;
}

.deal h3{
    font-size:18px;
    margin-bottom:8px;
}

.deal p{
    color:#388e3c;
    font-weight:bold;
}

/* ================= PRODUCT GRID ================= */

.products{
    display:grid;
    grid-template-columns:repeat(5,1fr);
    gap:15px;
}

.product{
    border:1px solid #eee;
    background:white;
    padding:15px;
    position:relative;
    transition:.25s;
}

.product:hover{
    transform:translateY(-5px);
    box-shadow:0 5px 20px #ccc;
}

.wishlist{
    position:absolute;
    top:12px;
    right:12px;
    width:35px;
    height:35px;
    border-radius:50%;
    background:white;
    box-shadow:0 1px 5px #ddd;
    font-size:20px;
    z-index:2;
}

.product-image{
    height:190px;
    display:flex;
    align-items:center;
    justify-content:center;
    font-size:105px;
}

.product h3{
    font-size:15px;
    line-height:1.4;
    min-height:43px;
    margin-bottom:8px;
}

.rating{
    background:#388e3c;
    color:white;
    padding:4px 7px;
    font-size:12px;
    border-radius:3px;
}

.price{
    font-size:20px;
    font-weight:bold;
    margin-top:9px;
}

.old-price{
    color:#888;
    text-decoration:line-through;
    font-size:13px;
}

.discount{
    color:#388e3c;
    font-size:13px;
    font-weight:bold;
    margin-left:5px;
}

.add-cart{
    width:100%;
    margin-top:12px;
    padding:11px;
    background:#ff9f00;
    color:white;
    font-weight:bold;
}

.buy{
    width:100%;
    margin-top:7px;
    padding:11px;
    background:#fb641b;
    color:white;
    font-weight:bold;
}

/* ================= BIG OFFER ================= */

.offer-banner{
    min-height:220px;
    background:linear-gradient(90deg,#172337,#2874f0);
    color:white;
    display:flex;
    align-items:center;
    justify-content:space-between;
    padding:30px 8%;
}

.offer-banner h2{
    font-size:35px;
    margin-bottom:10px;
}

.offer-banner p{
    font-size:18px;
    margin-bottom:20px;
}

.offer-btn{
    padding:13px 25px;
    background:#ff9f00;
    color:white;
    font-weight:bold;
}

.offer-art{
    font-size:120px;
}

/* ================= BRAND ================= */

.brands{
    display:grid;
    grid-template-columns:repeat(6,1fr);
    gap:15px;
}

.brand{
    border:1px solid #eee;
    min-height:110px;
    display:flex;
    align-items:center;
    justify-content:center;
    flex-direction:column;
    background:#fff;
}

.brand-icon{
    font-size:40px;
    margin-bottom:8px;
}

.brand strong{
    font-size:14px;
}

/* ================= FEATURES ================= */

.features{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:15px;
    margin:15px 0;
}

.feature{
    background:white;
    text-align:center;
    padding:28px 15px;
}

.feature-icon{
    font-size:45px;
    margin-bottom:10px;
}

.feature h3{
    margin-bottom:7px;
}

.feature p{
    color:#777;
    font-size:13px;
}

/* ================= NEWSLETTER ================= */

.newsletter{
    background:white;
    padding:30px;
    text-align:center;
    margin:15px 0;
}

.newsletter h2{
    margin-bottom:10px;
}

.newsletter p{
    color:#666;
    margin-bottom:20px;
}

.subscribe
