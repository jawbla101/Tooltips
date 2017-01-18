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
