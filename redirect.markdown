---
layout: default
title: Old Bob Gunpowder Redirect
permalink: /redirect
---
<p>Redirect, please wait...</p>
<script>
    var $_GET = {};
    if(document.location.toString().indexOf('?') !== -1) {
        var query = document.location
            .toString()
            .replace(/^.*?\?/, '')
            .replace(/#.*$/, '')
            .split('&');

        for(var i=0, l=query.length; i<l; i++) {
            var aux = decodeURIComponent(query[i]).split('=');
            $_GET[aux[0]] = aux[1];
        }
    }
    switch($_GET['to']){
        case 'album_oldbobgunpowder':
            window.location.replace("/album_oldbobgunpowder");
            break;
    }

</script>