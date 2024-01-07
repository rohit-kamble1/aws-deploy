# 
FROM python:3.9

# 
WORKDIR /python_projects

# 
COPY ./requirements.txt /python_projects/requirements.txt

# 
RUN pip install --no-cache-dir --upgrade -r /python_projects/requirements.txt

# 
COPY ./app /python_projects/app

# 
CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "80"] 