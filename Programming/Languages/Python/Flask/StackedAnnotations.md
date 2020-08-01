@app.route("/artist/<string:_id>", methods=["GET"], defaults={'limit': 0, 'order': "id", 'reverse': "False"})
@app.route("/artist/<string:_id>/<int:limit>", methods=["GET"], defaults={'order': "id", 'reverse': "False"})
@app.route("/artist/<string:_id>/<int:limit>/<string:order>", methods=["GET"], defaults={'reverse': "False"})
@app.route("/artist/<string:_id>/<int:limit>/<string:order>/<string:reverse>", methods=["GET"])
def artist(_id, limit, order, reverse):
    pass