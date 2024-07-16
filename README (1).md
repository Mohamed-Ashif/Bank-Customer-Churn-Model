
# CEBU-CDP-BACKEND

## Overview

This backend service is crafted for the CDP (Customer Data Platform) Module and built on Python and FastAPI. It provides secure authentication and efficient management of booker and passenger data. The service includes various endpoints for retrieving detailed information about passengers and bookers, enabling smooth data access and processing.








 


## API Endpoints

#### 1. Health Check

```http
GET /api/health
```

Checks if the service is up and running.

#### 2. Get Milestones

```http
GET /api/milestones
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `access_token`      | `string` | Your access token |

Fetches milestone data.

#### 3. Get Profile

```http
GET /api/profile
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `profile_type`      | `string` | **Required**: Specify 'passenger' or 'booker' |
| `id`      | `string` | **Required**: Id of the profile to fetch |
| `access_token`      | `string` | Your access token |

Fetches profile data for a passenger or booker based on the provided ID.

#### 4. Search Profile

```http
GET /api/profile/search
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `profile_type`      | `string` | **Required**: Specify 'passenger' or 'booker' |
| `firstname`      | `string` | Optional: First name to search |
| `lastname`      | `string` | Optional: Last name to search |
| `phone`      | `string` | Optional: Phone number to search |
| `email`      | `string` | Optional: Email address to search |
| `id`      | `string` | Optional: ID to search |
| `dateofbirth`      | `string` | Optional: Date of birth to search |
| `access_token`      | `string` | Your access token |

Searches profiles based on the provided criteria.

#### 5. Copy Files

```http
GET /api/copy_files
```

Synchronizes files from the specified S3 bucket to the local directory.







## Installation

- Clone the repository:

```bash
git clone https://github.com/Mindgraph-Cebu/CeBu-CDP-Backend.git

cd CEBU-CDP-BACKEND

```

* Create a virtual environment and activate it:

```bash
python -m venv myenv

source myenv/bin/activate

```

* Install the dependencies:

```bash
pip install -r requirements.txt

```

* Set up your environment variables in the .env file.

`TENANT_ID = your-tenant-id`

`BUCKET_NAME = your-bucket-name` 

`ATHENA_SCHEMA_NAME = your-athena-schema-name`

`S3_STAGING_DIR = your-s3-staging-directory`

`USER_ENV = your-environment  # 'athena', 'local', or 's3'`

## Usage

- Start the FastAPI server:

```bash
uvicorn main:app --reload

```

- Access the endpoints:

Access the endpoints via http://127.0.0.1:8000 in your web browser or API client.


  


## Authors

- Author: Pradish Pranam
- Copyright: MindGraph Technologies
- Version: 0.1.0
- Maintainers: 
  - Pradish Pranam
  - Mohamed Ashif H
- Email: 
  - pradishpranam.s@mind-graph.com
  - ashif.hm@mind-graph.com
- Status: Development
- Date: 04/Apr/2024



## License

- Copyright (c) 2024. MindGraph Technologies. All rights reserved.
- Proprietary and confidential. Copying and distribution is strictly prohibited.

