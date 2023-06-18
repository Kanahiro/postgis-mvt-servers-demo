wget https://nlftp.mlit.go.jp/ksj/gml/data/N03/N03-2023/N03-20230101_GML.zip
unzip N03-20230101_GML.zip
ogr2ogr -f PostgreSQL  postgresql://docker:docker@localhost/postgres N03-23_230101.shp -oo ENCODING=cp932