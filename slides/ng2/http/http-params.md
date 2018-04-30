## Passer des paramètres

    let params = new HttpParams();
    params = params.append('size', 20);
    return http.get<Session[]>(`/api/sessions`, { params });
