# Tooltips
hovering tooltips

spacings are a bit all over the place. it seems when i try to position the tooltip, the position spacing related to the parent container, not the element you are hovering over......
[18/01, 20:17] Alski Wolski: So first up your hover pseudo class should ideally be on the a in the css so you could do:
[18/01, 20:18] Alski Wolski: .rss a:hover::after { what you have already there}
[18/01, 20:20] Alski Wolski: Next you could have that content already there but hidden and then show it on hover
[18/01, 20:20] Alski Wolski: So:
[18/01, 20:21] Alski Wolski: .rss a::after { what you have + a display:none;}
[18/01, 20:22] Alski Wolski: Then:
[18/01, 20:22] Alski Wolski: .rss a:hover::after { display:block; }
[18/01, 20:24] Alski Wolski: That's an enhancement anyhoo, so is putting the common styles in a more generic selector like li a { position: absolute;}
[18/01, 20:25] Alski Wolski: And finally, you need a position:relative; on the li tags there
[18/01, 20:25] Alski Wolski: Or the as
