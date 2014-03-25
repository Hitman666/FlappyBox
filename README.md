FlappyBox
=========

This is basically just an addition to the great 3 series tutorial ([part 1](http://blog.lessmilk.com/how-to-make-flappy-bird-in-html5-1/), [part 2](http://blog.lessmilk.com/how-to-make-flappy-bird-in-html5-2/), [part 3](http://blog.lessmilk.com/how-to-make-flappy-bird-in-html5-3/)) from [LessMilk's blog](http://blog.lessmilk.com/) and hereby I thank him for them.

The original tutorial makes the bird (square) jump by pressing the space key, whilst to make the bird jump on a mouse click (or tap on mobile devices) all you have to do is replace the

`var space_key = this.game.input.keyboard.addKey(Phaser.Keyboard.SPACEBAR);`

in the menu.js  file with:

`var space_key = this.game.input;`

Also, I added the crash sound (original file from here) in the hit_pipe  function:

`if (this.bird.alive == false){
    this.crash_sound.play();
    return;
}`

which I've defined in the create function:

`this.crash_sound = this.game.add.audio('crash');`

of the file play.js .

You can try the game [here](http://nikola-breznjak.com/_testings/phaser/flappy_bird/).
