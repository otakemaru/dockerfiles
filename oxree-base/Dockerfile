FROM otakemaru/passenger-ruby22:5.0.23
RUN apt-get update \
  && apt-get install -y wkhtmltopdf unzip \
  && apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
RUN mkdir -p /home/app/.font \
  && cd /home/app/.font \
  && curl \
    --location \
    --silent \
    --retry 3 \
    --remote-name \
    "http://dl.ipafont.ipa.go.jp/IPAexfont/ipaexg00301.zip" \
  && unzip ipaexg00301.zip \
  && rm -f ipaexg00301.zip

