## Exam instruction

* Using the data/json on `instructions\data.json`, sample structure below:
```json
{
	"items":
		{
			"item":
				[
					{
						"id": "0001",
						"type": "donut",
						"name": "Cake",
						"ppu": 0.55,
						"batters":
							{
								"batter":
									[
										{ "id": "1001", "type": "Regular" },
										{ "id": "1002", "type": "Chocolate" },
										{ "id": "1003", "type": "Blueberry" },
										{ "id": "1004", "type": "Devil's Food" }
									]
							},
						"topping":
							[
								{ "id": "5001", "type": "None" },
								{ "id": "5002", "type": "Glazed" },
								{ "id": "5005", "type": "Sugar" },
								{ "id": "5007", "type": "Powdered Sugar" },
								{ "id": "5006", "type": "Chocolate with Sprinkles" },
								{ "id": "5003", "type": "Chocolate" },
								{ "id": "5004", "type": "Maple" }
							]
					},
					...
				]
		}
}
```
* Create a sortable table - showing all available data sets possible. The `instructions\data.json` dataset should render something similar below:
![alt text](https://raw.githubusercontent.com/cenon4dno/generator-angular-library/master/instructions/demo.png)
* Clicking the column header should sort the table. Example clicking `id` should sort the entire table base on their id.
* Additional task is to add an input box above the table, that will filder the `name`. (e.g. If I type `Raised` it should only show all the rows with `name` equal to `Raised`)
