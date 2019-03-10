FROM continuumio/anaconda3

# copy source code in (only used in production volume used in local development)
COPY ./ /var/www

# install gunicorn to serve the flask app
RUN pip install gunicorn

WORKDIR /var/www/MovieReviewClassifier

CMD ["gunicorn"  , "-b", "0.0.0.0:5000", "MovieReviewPredict:app"]