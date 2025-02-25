# CS361
To request data:
    -> write to 'inventory.txt' in the format:
            item_id: <item_id>, stock: <current_stock>, threshold: <threshold>
    -> example call:
            with open('inventory.txt', 'w') as file:
                file.write('item_id: 201, stock: 2, threshold: 5')

To recieve data:
    -> to receive alerts, read from 'alerts.txt':
            with oepn('alerts.txt', 'r') as file:
                alerts = file.readlines()
                for alert in alerts:
                    print(alert.strip())

UML
![UML Sequence Diagram](./images/UML.jpg)
