# grapghql
	pour recuppéer la liste de compte:
			query {
				accountList{
					id
				}
			}

	pour recuperer une seule elemenet:
			query {
				accountById(id: "8326eabb-add1-4405-914e-ab12fe25c1cd") {
				balance
			} 
			}
   
   	pour ajouter un elemenet:
			mutation {
			  addAccount(account: {
			    type: "SAVING_ACCOUNT",
			    balance: 4000,
			    currency: "USD"
			  }) {
			    id, type, balance
			  } 
			}

   ![image](https://github.com/user-attachments/assets/0ebc4afe-b286-4d10-8124-21b6e9a81a29)

			mutation ($type: String, $balance: Float, $currency: String ){
			  addAccount(account: {
			    type: $type,
			    balance: $balance,
			    currency: $currency
			  }) {
			    id, type, balance
			  } 
			}

   			dans variable: 
			{
			  "type": "SAVING_ACCOUNT",
			  "balance": 5000, 
			  "currency":  "USD"
			}
