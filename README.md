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
