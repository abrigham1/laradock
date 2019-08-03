FROM continuumio/anaconda3

# install gunicorn to serve the flask app
RUN /opt/conda/bin/conda install -c anaconda gunicorn

#install flask
RUN /opt/conda/bin/conda install -c anaconda flask

# install flask-cors
RUN /opt/conda/bin/conda install -c anaconda flask-cors

WORKDIR /var/www/MovieReviewClassifier

CMD ["/opt/conda/bin/gunicorn"  , "-b", "0.0.0.0:5000", "MovieReviewPredict:app"]
