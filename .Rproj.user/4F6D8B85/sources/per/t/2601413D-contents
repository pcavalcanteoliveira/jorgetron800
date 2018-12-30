### botzera regular

library(twitteR)
library(vagalumeR)
library(tibble)
library(stringr)
set.seed(1234)

consumerKey = 'jIhYluFluZvG9eg7rw4IWr65p'
consumerSecret = 'nAMRBixi3HvM01nHcyLRC0wDtubi9flVvDEc9RQW58kOQZz7Ru'
accessToken = '1079161008986427393-mfKbK0DYeC7EFIlC4oOSNQj38KPzRw'
accessTokenSecret = 'TFO4njpN9u8hGWnCjQUKvIRNovDwf9aP1npaNfelp3u2O'

key = "7a67715b6d0dd6edf7556cc0d176e4ac"

#Connect to twitter
setup_twitter_oauth(consumerKey, 
                    consumerSecret,
                    accessToken,
                    accessTokenSecret)

musicas = as.tibble(topLyrics(name = "seu-jorge",
                              message = TRUE))

musica = sample(musicas$id.top, 1)

letra = lyrics(identifier = musica,
       type = "id",
       artist = "seu-jorge",
       key = key)

letra = str_split(string = as.character(letra), "(?=[[:upper:]])")
letra = letra[[6]]

inteiros = seq(from = 6, to = length(letra))

indice = sample(inteiros, 1)

if(nchar(letra[indice]) > 1) {
  
  tweet = paste(letra[indice],
                letra[indice+1],
                letra[indice+2])

  } 
   if(nchar(tweet) > 140) {

    tweet = paste(letra[indice],
                letra[indice+1])
  
    } else {
  
      tweet = paste(letra[indice],
                    letra[indice+1],
                    letra[indice+2],
                    letra[indice+3])
}

tweet(tweet)
       
