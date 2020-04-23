### botzera regular

library(dplyr)
library(dplyr)
library(glue)
library(twitteR)
library(dotenv)
library(lubridate)

now() %>%
  as.numeric() %>%
  set.seed()

load_dot_env(".env")
source("C:/Users/cavap/Desktop/Cava/jorgetron800/insumos.R")

setup_twitter_oauth(consumer_key = Sys.getenv("consumerKey"), 
                    consumer_secret = Sys.getenv("consumerSecret"),
                    access_token = Sys.getenv("accessToken"),
                    access_secret = Sys.getenv("accessTokenSecret"))

(tweet <- glue("{sample(Sujeito, 1)} aproveita {sample(Objeto, 1)} para defender {sample(projeto, 1)}"))

tweet(tweet)
