FROM continuumio/anaconda3

# install gunicorn to serve the flask app
RUN pip install gunicorn

WORKDIR /var/www/MovieReviewClassifier

CMD ["gunicorn"  , "-b", "0.0.0.0:5000", "FlaskTest:app"]