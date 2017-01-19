# Tooltips
hovering tooltips

spacings are a bit all over the place. it seems when i try to position the tooltip, the position spacing related to the parent container, not the element you are hovering over......
</br>[18/01, 20:17] Alski Wolski: So first up your hover pseudo class should ideally be on the a in the css so you could do:
</br>[18/01, 20:18] Alski Wolski: .rss a:hover::after { what you have already there}
</br>[18/01, 20:20] Alski Wolski: Next you could have that content already there but hidden and then show it on hover
</br>[18/01, 20:20] Alski Wolski: So:
</br>[18/01, 20:21] Alski Wolski: .rss a::after { what you have + a display:none;}
</br>[18/01, 20:22] Alski Wolski: Then:
</br>[18/01, 20:22] Alski Wolski: .rss a:hover::after { display:block; }
</br>[18/01, 20:24] Alski Wolski: That's an enhancement anyhoo, so is putting the common styles in a more generic selector like li a { position: absolute;}
</br>[18/01, 20:25] Alski Wolski: And finally, you need a position:relative; on the li tags there
</br>[18/01, 20:25] Alski Wolski: Or the as
</br><b>still cant get this friggin thing working. i reallythink that there must be a referenced css file in the html thats screwing my css up - hence the text not being displayed in the tool tips. The text is present because when i change the content, the tool tip changes size to accomodate it!</b>
</br>Also the tooltip is disappearing behind the containing div and i cant for the life of me figure out why!

