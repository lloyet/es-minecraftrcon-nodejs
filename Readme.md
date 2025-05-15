# Api Minecraft RCON

Minecraft RCON API to send raw minecraft nvms commandes via http requests.

## Quickstart

```sh
# Installer dependencies
npm ci

# Start application
npm run dev
```

## Documentation

## 📦 Endpoints disponibles

| Méthode | Route      | Description                           |
| ------: | ---------- | ------------------------------------- |
|     GET | `/`        | Healthcheck                           |
|    POST | `/rcon`    | Send RAW Minecraft nvms command lines |
|     GET | `/version` | Get API current version               |

---

## [GET] `/`

Verify health of application.

**Response**

```sh
OK
```

## [GET] `/versions`

GET curretn version of API.

**Response**

```json
{
  "version": "1.0.0"
}
```

## [POST] `/rcon`

Send RAW Minecraft nvms command lines using body as `JSON`.

**Request**

```json
{
  "command": "say hello"
}
```

**Response**

```json
{
  "message": "hello"
}
```
