# Neighborhood-Associations-Parser


In the core/settings.py file:
1. The "/Neighborhood-Associations-Export.zip" must be changed to match the Caspio zip filename that will be exported
    >> export_file = Path(str(export_path) + "/Neighborhood-Associations-Export.zip")
2. The "/Neighborhood_table.csv" must also be changed to match the Caspio zip filename that will be extracted
    >> file = Path(str(export_path) + "/Neighborhood_table.csv")

In the core/database.py file:
1. Create a core/database.py

    import MySQLdb


    # Database connection
    db_connection = MySQLdb.connect(
        host="hostname",
        user="username",
        passwd="password",
        database="databasename"
    )