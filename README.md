# bearer-auth

## LAB - 07

### Deployment Test


- [ci/cd GitHub Actions](https://github.com/MohammadAljadayh/basic-auth/actions).
- [herokuapp Link Main ](https://mohammadbasicauth.herokuapp.com/).
-[PULL_REQUEST ](https://github.com/MohammadAljadayh/basic-auth/pull/1).
- [PULL_REQUEST ](https://github.com/MohammadAljadayh/basic-auth/pull/2).
- [Main Repo link](https://github.com/MohammadAljadayh/basic-auth).

### Setup 

`.env` **requirements**

- `PORT` - 3000

- `DATABASE_URL` = Postgres DB
- - `SECRET` = JWT SECRET 

**Running the app**

- `npm start`

- Endpoint: `/signup`
```
 { 
    "username": "root" ,
     "password": "root" 
     
     }
```
- Returns : 
```
{
  {
    "user": {
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6InJvb3QxIiwiaWF0IjoxNjM2Mzk2Njg2fQ.IVWLalj07KcDqt_8CAH9SgO-haAdKUOx4YytNYXz-BY",
        "id": 54,
        "username": "root1",
        "password": "{}",
        "updatedAt": "2021-11-08T18:38:06.408Z",
        "createdAt": "2021-11-08T18:38:06.408Z"
    },
    "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6InJvb3QxIiwiaWF0IjoxNjM2Mzk2Njg2fQ.IVWLalj07KcDqt_8CAH9SgO-haAdKUOx4YytNYXz-BY"
}

```
- Endpoint: `/signin`

> Username `root`
> Password `root`

- Returns 
```
{
    "id": 2,
    "username": "root",
    "password": "$2b$10$crd318T2i747Lph8kGGwO.W8X4/YKkWhzPSfWjI/7jlRVpAe9QDfa",
    "createdAt": "2021-11-07T15:31:59.924Z",
    "updatedAt": "2021-11-07T15:31:59.924Z"
}
```

- Endpoint: `/users`


**Tests**

- Unit Tests: `npm run test`
- Lint Tests: `npm run lint`

![UML](uml.PNG)
