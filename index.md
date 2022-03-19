# Hope you're having a good day
![](https://i0.wp.com/brightestyoungthings.com/wp-content/uploads/2016/02/150754-bears-waving-gif-imgur-tumblr-jfGo.gif?fit=410%2C220&quality=100&ssl=1)

## Some things about me
* I'm currently doing a BSc at the University of Auckland, majoring in Statistics.
* I'm **terrible** with planning in advance and am unpredictable so I might change majors in the future, or I might not.
* I like telling people about my interests, so I **will** force my incoherent babblings on the nearest person.
* I have many interests such as ![anime](https://en.wikipedia.org/wiki/Anime), reading 📖, and listening to music 🎼.

## The meme you've been waiting for:
![](mymeme.png)

__The code for the meme:__
```
library(magick)

##code for panel row 1 text
panel1 <- image_blank(width = 500,
                      height = 340,
                      color = "#000000") %>%
  image_annotate(text = "working out in\nspring/autumn",
                 color = "#FFFFFF",
                 size = 40,
                 font = "Impact",
                 gravity = "center")

##row 2 text
panel2 <- image_blank(width = 500,
                          height = 310,
                          color = "#000000") %>%
  image_annotate(text = "working out in\nwinter/summer",
                 color = "#FFFFFF",
                 size = 40,
                 font = "Impact",
                 gravity = "center")

##images
happy_runner <- image_read("https://media.istockphoto.com/photos/happy-female-runner-jogging-in-the-morning-in-nature-picture-id1142900322?k=20&m=1142900322&s=170667a&w=0&h=ZMKkYqci_krlhBKRLFOLnEHK9sBA_xleNtsIW3APp_c=")

not_happy <- image_read("https://happymag.tv/wp-content/uploads/2021/08/F-14.jpg") %>%
  image_scale(510)

#row1 image with text

row1<- c(happy_runner, panel1) %>%
  image_append()


#row2 image with text

row2 <- c(not_happy, panel2) %>%
  image_append()

##incorporated
meme <- c(row1, row2) %>%
  image_append(stack = T)

image_write(meme, "mymeme.png")
```

### An explanation for the meme.
1. I like exercising :muscle:.
2.  I like telling people about my interests.
3.  This meme format is _fairly typical_ and is also a good way to let as many people as possible know that I like working out.
4.  I find it hard to get started in winter and summer though, since:
> * lying in bed is so much easier than going into the cold to work out
> * I get sweaty working out in summer :rage:
 
 Thank you for visiting :)
 
 ![](https://c.tenor.com/aMTgGRQyqBUAAAAC/animal-crossing-tom-nook.gif)
 
