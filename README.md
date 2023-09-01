# Dokumentasi API RESTful Task

Dokumentasi ini menjelaskan penggunaan API RESTful sederhana untuk mengelola daftar tugas (tasks) menggunakan Laravel.

## Prasyarat

-   Laravel sudah terinstal di sistem Anda. Jika belum, Anda dapat mengikuti panduan instalasi di [Laravel Documentation](https://laravel.com/docs/).

## Penggunaan API

### Menampilkan Daftar Tugas (GET /api/tasks)

-   **Deskripsi**: Mendapatkan daftar semua tugas.
-   **Metode**: GET
-   **URL**: `/api/tasks`   
-   **Contoh Permintaan**: `GET /api/tasks`
-   **Contoh Respons Sukses**:
    ```json
    [
    	{
    		"id": 1,
    		"title": "Tugas Pertama",
    		"description": "Deskripsi Tugas Pertama",
    		"created_at": "2023-09-01T12:34:56.000000Z",
    		"updated_at": "2023-09-01T12:34:56.000000Z"
    	},
    ]
    ```
