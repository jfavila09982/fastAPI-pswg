FROM python:3.10.6

# 
WORKDIR /code

# 
COPY ./requirements.txt /code/requirements.txt

# 
RUN pip install --no-cache-dir --upgrade -r /code/requirements.txt

# 
COPY ./app /code/app


# Use an environment variable to specify the port to listen on
CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8085"]
