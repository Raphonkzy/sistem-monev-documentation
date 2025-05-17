# /password

Endpoint ini digunakan untuk reset password.

## POST /authentication/register

### Body

```
{
    "email": "urEmail@mail.com"
}
```

### Response

```
{
    "status": "success",
    "message": "Kode reset password berhasil dikirim melalui email"
}
```

## PUT /authentication/password

### Body

```
{
    "email": "urEmail@mail.com",
    "resetCode": "urResetCode",
    "newPassword": "urNewPassword",
    "confirmPassword": "urNewConfirmedPassword"
}
```

### Response

```
{
    "status": "success",
    "message": "Password berhasil direset"
}
```