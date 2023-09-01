# Dokumentasi API RESTful Task

Dokumentasi ini menjelaskan penggunaan API RESTful sederhana untuk mengelola daftar tugas (tasks) menggunakan Laravel.

## Prasyarat

-   Laravel sudah terinstal di sistem Anda. Jika belum, Anda dapat mengikuti panduan instalasi di [Laravel Documentation](https://laravel.com/docs/).

## Penggunaan API

### Menampilkan Daftar Tugas (GET /api/tasks)

-   **Deskripsi**: Get list all data task.
-   **Metode**: GET
-   **URL**: `/api/tasks`
-   **Contoh Respons Sukses**:

    ```json
    [
    	{
    		"id": 1,
    		"title": "Tugas Pertama",
    		"description": "Deskripsi Tugas Pertama",
    		"created_at": "2023-09-01T12:34:56.000000Z",
    		"updated_at": "2023-09-01T12:34:56.000000Z"
    	}
    ]
    ```

-   **Deskripsi**: Get detail data task.
-   **Metode**: GET
-   **URL**: `/api/tasks/{id}`
-   **Contoh Respons Sukses**:
    ```json
    {
        "id": 1,
        "title": "Tugas Pertama",
        "description": "Deskripsi Tugas Pertama",
        "created_at": "2023-09-01T12:34:56.000000Z",
        "updated_at": "2023-09-01T12:34:56.000000Z"
    }
    ```

-   **Deskripsi**: Create data task.
-   **Metode**: POST
-   **URL**: `/api/tasks`
-   **Body**: 
    ```json
    {
        "title": "Task 1",
        "description": "Description of Task 1",
    }
    ```
-   **Contoh Respons Sukses**:
    ```json
    {
        "message": "Task created successfully"
    }
    ```

-   **Deskripsi**: Update data task.
-   **Metode**: POST
-   **URL**: `/api/tasks/{id}`
-   **Body**: 
    ```json
    {
        "title": "Task edit",
        "description": "Description of Task edit",
    }
    ```
-   **Contoh Respons Sukses**:
    ```json
    {
        "message": "Task updated successfully"
    }
    ```

-   **Deskripsi**: Detete data task.
-   **Metode**: DETETE
-   **URL**: `/api/tasks/{id}`
-   **Contoh Respons Sukses**:
    ```json
    {
        "message": "Task deleted successfully"
    }
    ```
