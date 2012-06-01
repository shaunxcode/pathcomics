#PathComics
##What?
An online interactive comic editing system mainly targeted at people interested in creating "choose your own adventure" comics with recurring scenes/characters. Each scene will be scriptable via a visual drag and drop programming language (blockly). Currently the scripting will be things like "on click play this sound" or "on click go to this other scene" but in theory animation etc. will be possible at some future point. The goal is to provide an embeddable comic that you can put on your wordpress, social media outlet of choice etc. There is also the notion of the direct link to the comic so it can be viewed on pathcomics.com itself. Sharing and forking of universes will be encouraged but not required e.g. you can set whether you want your universe to be "forkable" or "shareable" (characters, props, costumes, scenery)

##How? 
coffeescript, socket.io, express.js, blockly, raphael.js


##What does it look like?
A big draggable canvas where scenes can be positioned as they make sense to the artist. This could be a big tile grid or a jumble of crazy. Totally up to the user. I imagine providing some positioning options like "tile" or "group by relation" could be beneficial but hardly a requirement. 

When a user clicks on a scene they will have buttons (edit, delete, clone). If they click edit they will open a larger version of the scene which allows them to edit the multiple layers by placing content on the layers and then scripting actors/actions. 

When scripting a scene the user will have a toolbox filled with the names of all of the items in their scene (actors, props, arbitrary clickable polygons they have drawn) with which they can drag to the scripting area and plug into the various blocks. 

##Why?
Because providing a platform for expression seems like a good thing to do. 

##Licensing? 
MIT. Use it how ever you like. Ideally pathcomics.com will become some sort of hub for sharing universes and ideas but ultimately if you want to download it and run your own server thats sweet to. In fact the whole thing is going to be published as an npm package so you literally just need to run ```npm install pathcomics``` and then ```pathcomics-server``` and hit ```http://localhost:6055``` in your browser to start playing around. 