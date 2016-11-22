# TablesQuery

**TablesQuery** - ��� ���� ��������, �������������� ���������� ��� StoryCLM. 
������ � ������ ������� ����� ������������� � ���� ������ ����� ��������. ��������� �� ������� ��������� ������ ����� ���� ���� �����: Comparison � Logical. 

### Comparison (��������� ���������):

�������� |	��� ���� ��� �������� �� ��������     |	������ �������	              | ��������
---------|----------------------------------------|-------------------------------|---------------------------
[eq]	 | (string, int, double, bool, date)	  | [fieldname][eq]["value"]	  | Equals
[lt]	 | (int, double, date)	                  | [fieldname][lt][value]	      | Less Than operator
[lte]	 | (int, double, date)	                  | [fieldname][lte][value]	      | Less Than or Equal to operator
[gt]	 | (int, double, date)	                  | [fieldname][gt][value]	      | Greater Than operator
[gte]	 | (int, double, date)	                  | [fieldname][gte][value]	      | Greater Than or Equal to operator
[ne]	 | (string, int, double, bool, date)	  | [fieldname][ne]["value"]      | Not Equal to operator
[in]	 | (string, int, double, bool, date)	  | [fieldname][in]["val","val"]  |	Contained IN array operator
[nin]	 | (string, int, double, date)	          | [fieldname][nin]["val","val"] |	Not contained IN array
[cn]	 | (string)	                              | [fieldname][cn]["value"]	  | Contains
[re]	 | (string)	                              | [fieldname][re]["value"]	  | Regular Expression
[sw]	 | (string)	                              | [fieldname][sw]["value"]	  | Starts With
[ew]	 | (string)	                              | [fieldname][ew]["value"]	  | Ends With

### Logical (���������� ���������): 

������������ ��� "����������" ��������� ���������� ��������� ���������� ���������. ����� ��������� ����� ������������� ������ ����� ����������� ���������. ��������� ��������� ������� � ������ ������, � �����, ����������� ������ ���������� ���������, ����������� ���������� �������� � �������� ��������� ����������� �� �����.

��������  |	��� ���� ��� �������� �� ��������	| ������ �������
----------|-------------------------------------|--------------------------------------
[or]	  |(���������� ��������)	            | [fieldname][eq]["value"][or][fieldname][eq]["value1"]
[and]	  |(���������� ��������)	            | [fieldname][eq]["value"][and][fieldname][eq]["value1"]