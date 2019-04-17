FROM continuumio/anaconda3

# install gunicorn to serve the flask app
RUN conda install -c anaconda gunicorn

#install flask
RUN conda install -c anaconda flask

# install flask-cors
RUN conda install -c anaconda flask-cors

WORKDIR /var/www/MovieReviewClassifier

CMD ["gunicorn"  , "-b", "0.0.0.0:5000", "MovieReviewPredict:app"]