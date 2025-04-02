I began studying math and the factorization problem back in the summer of 2023. 
Not having achieved higher education, I had the learn everything from the ground up.
The paper and proof of concept are the result of one year of work. The paper is very flawed due to my at the time limited understanding. (i.e things such as the "rebasing" step are not needed, since they are already congruent mod p)

However, representing factorization as Quadratic coefficients, despite my many other flaws, did turn out to be a very good appraoch.

This repro has a collection of PoCs. Including the original paper from august 2024, and an attempt to solve it with LLL.
The latest version QS.py will factor 150 bit keys in a few minutes, useage:

python3 QS.py -keysize 150

My final version will be released soon. I struggled for a while to connect all these findings. But today (2 april), after an especially shitty day where I really just wanted to die, it finally came to me, as it always does in my darkest hours.
There was this really fundemental number theoretical trick I wasn't applying due to my inexperience, but with that figured out, it finally clicked. How I can connect quadratic coefficients on both sides of the congruence so I don't need to brute force them... which was the very last thing I had to figure out to conclude this 2 year project.
