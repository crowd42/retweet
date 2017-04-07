[<img src="https://api.travis-ci.org/chaica/retweet.svg?branch=master">](https://travis-ci.org/chaica/retweet)
### Retweet 

Retweet automatically retweets tweets from a Twitter user. Read the documentation in docs/
or [read it online](https://retweet.readthedocs.org/en/latest/).

If you would like, you can [support the development of this project on Liberapay](https://liberapay.com/carlchenet/).
Alternatively you can donate cryptocurrencies:

- BTC: 1BcdXCcLKN9PRpp6qw23FYkYuVp59dKZix
- XMR: 4Cxwvw9V6yUehv832FWPTF7FSVuWjuBarFd17QP163uxMaFyoqwmDf1aiRtS5jWgCiRsi73yqedNJJ6V1La2joznUDzkmvBr6KKHT7Dvzj

### Quick Install

* Install Retweet from PyPI

        # pip3 install retweet

* Install Retweet from sources    
  *(see the installation guide for full details)
  [Installation Guide](http://retweet.readthedocs.org/en/latest/install.html)*
  

        # tar zxvf retweet-0.10.tar.gz
        # cd retweet
        # python3 setup.py install
        # # or
        # python3 setup.py install --install-scripts=/usr/bin

### Use Retweet

* Create or modify retweet.ini file in order to configure Retweet:

        [twitter]
        screen_name_of_the_user_to_retweet=journalduhacker
        consumer_key=ml9jaiBnf3pmU9uIrKNIxAr3v
        consumer_secret=8Cmljklzerkhfer4hlj3ljl2hfvc123rezrfsdctpokaelzerp
        access_token=213416590-jgJnrJG5gz132nzerl5zerwi0ahmnwkfJFN9nr3j
        access_token_secret=3janlPMqDKlunJ4Hnr90k2bnfk3jfnwkFjeriFZERj32Z

        [retweet]
        retweets=0
        waitminsecs=60
        waitmaxsecs=600
        do_not_retweet_hashtags=dnr,
        only_if_hashtags=python,
        match=[Rr]egex
        like=true

        [sqlite]
        sqlitepath=/var/lib/retweet/retweet.db

* Launch Retweet

        $ retweet /path/to/retweet.ini

### Authors

Carl Chenet <chaica@ohmytux.com>

### License

This software comes under the terms of the GPLv3+. See the LICENSE file for the complete text of the license.
