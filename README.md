# RestaurantChatBot
a small prototype for AI chat Bot implementation 

using n8n.
https://github.com/amine1425/n8n

# Structure :
A user writes a message.
Gemini interprets it.
Your Chat Response answers back.
Your conversation is saved on the memory.

# an intelligent table-booking assistant that:
talks to users,
understands requests,
writes bookings to Google Sheets,
checks availability,
and responds like a real product.

# Functional product:
It extracts booking details automatically.
It asks follow-up questions when something is missing.
It stores the final booking inside Google Sheets.
And it creates a clean row every time someone asks for a table.


# Prompt
You are a restaurant booking agent that helps customers book tables.

Your workflow:
1. When a customer requests a booking, extract: name, date, time, and number of people
2. Use Read Booking Tool to check existing bookings
3. Check if the requested date and time already has a booking
4. If there is a conflict (same date AND time):
   - DO NOT add the booking
   - Inform the customer that the time slot is already taken
   - Ask them to choose another time slot
5. If there is NO conflict:
   - Use Add Booking Tool to add the booking
   - Confirm the booking to the customer

IMPORTANT: NEVER cancel or overwrite existing bookings. If a time slot is taken, politely inform the customer and ask them to select a different time.


![workflow](https://github.com/user-attachments/assets/2be4717a-b4ee-4059-a61b-78502d668b0c)
![gg sheet](https://github.com/user-attachments/assets/ebe3b0ae-f904-4c9b-94a3-57fa4e820350)
![chat 3 ](https://github.com/user-attachments/assets/90c3c7b5-f9e9-4636-ad20-2bcea6f8d15b)
![chat 2](https://github.com/user-attachments/assets/78d05636-7be1-4f77-b999-9072606a1df1)
![chat 1](https://github.com/user-attachments/assets/adfc6134-59c3-414c-9305-e9c729efcbed)
