### botzera regular

library(twitteR)
library(vagalumeR)
library(tibble)
set.seed(1234)

consumerKey = 'jIhYluFluZvG9eg7rw4IWr65p'
consumerSecret = 'nAMRBixi3HvM01nHcyLRC0wDtubi9flVvDEc9RQW58kOQZz7Ru'
accessToken = '1079161008986427393-mfKbK0DYeC7EFIlC4oOSNQj38KPzRw'
accessTokenSecret = 'TFO4njpN9u8hGWnCjQUKvIRNovDwf9aP1npaNfelp3u2O'

#Connect to twitter
setup_twitter_oauth(consumerKey, 
                    consumerSecret,
                    accessToken,
                    accessTokenSecret)


musicas = as.tibble(topLyrics(name = "seu-jorge",
                              message = TRUE))


for(i in 1:nrow(musicas)) {

  musicas$index[i] = rnorm(n = 1)

}

musica = sample(musicas$id, 1)

lyrics(identifier = musica,
       type = "id",
       api = )




