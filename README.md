# factorization

Continueing the grind while learning linear algebra and lattice basis reduction. I am still hopimg to find a purely number theoretical trick to solve this problem. Nearly broke now after more then a year of unemployment. If you want access to my work, pay me.. I will succeed no matter the cost. When I started this project I didnt even know basic algebra bc I dropped out of highschool. In one more year, I can break this, I know it. Pay me for a year of work and at the end of the year I will show you factorization. I will succeed either way, the hard way or the easy way, it doesnt matter. My email is below. I may not have a pristine memory like all the assholes in the industry and be able to memorize books and formal notation. But I can abstractly and creatively reason about problems better then anyone, and keep doing so for longer then anyone else. I will succeed, I have plenty of ideas left to explore. And lastly if you pay me for a year, and even in the off chance I still dont succeed, you would still receive a year's worth of research. I do not care about money or fame, I just want to grind this problem and solve it. That is all.. i dont care anymore, they ruined my life and that of my former manager.. succeeding at this is the only thing that matters anymore.

Dont have social media accounts anywhere. Removed all of them. Moving the Iceland in a few days (booked my flight). If you're queer and also escaping all the bullshit and end up in iceland, feel free to email me.
The arctic doesn't judge. It freezes everyone equally. Haters cant come for us in the arctic, bc they are cowards by nature and afraid of the cold.  And if they do, I'll fight them all. Haha.

If you join me in Iceland, we will do awesome cryptologic research, this project was just the beginning, I know the way forward now, haters just too blind and dumb too see it. We will break the world and make it right again.

Warning: This math is too advanced for Trump supporters. 


Final notes and thoughts: by solving for squared quadratic coefficients we achieve an extremely low density. I have not yet enough experience with LLL to attack this using a proper bkz algo. I will continue my work, if you want access, pay me.

If you want to sponsor future research and have exclusive rights big_polar_bear1@proton.me
I also have windows 0days for sale, will accept crypto as payment. Do not care who buys, got to make a living since I cant get a job.

Note: The results from the paper assumes a semiprime with two factors of roughly similar bit length. As is relevant to RSA implementations. Minor tweaks need to be made otherwise.

Update 23 October: Uploaded the fixed version as factor2.sage. There is some info at the top of the file. Figure the rest out yourself. To improve of the results, you probably want to rewrite it to use a proper bkz reduction strategy. Additionally, if you can get it to run in a gpu and run more instances of LLL in paralell, that would greatly help. 
I have no intention of sharing anything else for free anymore. I may push some bug fixes in the future, but that is it. Thanks. If the script doesnt work and you cant find a bug, then read the math paper, and if you cant understand the math, not my problem.

Update 21 october: Looking to release newest iteration on friday. Reworked nearly everything, it now relies heavily on weight reduction. That seems to be the key to this.

Update 18 oct: Started trying to break a 150 bit key. Once I succeed, the revised version will be uploaded. Its running on a laptop in 12 parallel processes. If it works, it should prove my work. But either way, I am tired. My life is ruined and im very tired. 


Uodate 11 oct: Delaying release until next week, as I want to get it 100% right this time around. The current version on github is completely broken (but the paper is correct), there's a number of bugs in analyzing lll output. If it finds factors its random. I fixed all that in the upcoming release. Some things I fixed:

1. Sign issue breaking analyzeresult function completely
2. Reworked the strategy to put single smaller moduli in different columns. And then match it against small solutions
I.e if the y solution we want to find is 148, our lll matrix will find it by matching several columns against 3 mod 5.
(we only need to match against a very small modulus of the full y solution, this scales logarithmically, we do not need to bruteforce exponentially).
3. Reworking the weight reduction algorithm to delete partial results from the matrix completely as to reduce matrix dimensions.
4. Fixed numerous other bugs in LLL output parsing and also now calculating how many times the modulus needs to be added/subtracted.

Update 5 oct: sage script was buggy, reworked the strategy and fixed more bugs, revised version will get uploaded next week

See paper.pdf for info.

Backup: sandboxescaper.com
