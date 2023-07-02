Sin
===

* [Bhaskara I's sine approximation formula](https://en.wikipedia.org/wiki/Bhaskara_I%27s_sine_approximation_formula)
    * https://twitter.com/KilledByAPixel/status/1668498488408014850
        * > Today I learned about an approximation for sine discovered by Bhaskara in 600 CE. I am using it to fix tiny discrepancies with Math.sin in different browsers. Here's my code... #javascript #math #generativeart 
        * `Z=x=>(((x%=360)<0?x+=360:x)<180?4:-4)*(x=(x%=180)*(180-x))/(40500-x)`
        * > I should add this is LESS accurate then calling Math.sin(), with a maximum error of about 1.8% But it's small enough to not be visually noticeable, and for my use case the more important thing is that the results are exactly the same in different environments.
        * > Very nice! Consider also replacing `((x%=360)<0?x+=360:x)<180` with `(x=(x%360+360)%360)<180` or (depending on input range) `(x=(x+36e3)%360)<180`.
        * > Very tiny errors that can add up with some algorithms to eventually produce big differences in generative artwork. I am not sure why the cause but my guess is a slightly different size lookup table or slightly different method of interpolation.
