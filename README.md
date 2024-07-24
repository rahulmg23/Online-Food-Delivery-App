link live demo - https://food-delivery-nine-psi.vercel.app
# Online-Food-Delivery-App
    ### Technology
    
    - React
    - Spring boot
    - spring security
    - role base access (ROLE_CUSTOMER, ROLE_RESTAURANT_OWNER)
    - spring start mail
    - jeson web token
    - Mysql(Data base)
    - Tailwind css
    - Mui (css component library)
    - Redux (State managment library)
    - Axios
    - strip payment gatway
    
    ### Tools
    
    - intellij idea (spring boot)
    - vs code (react)

link - https://food-delivery-nine-psi.vercel.app/
**

### Tools

- vs code (react)

- Model
    - User
        
        # User Entity
        
        ```jsx
        
        	Long id;
        	fullName;
        	email;
        	password;
        	role;
        	orders;
        	favorites
        	addresses 
        	status;
        ```
        
    - Restaurant
        
        ```jsx
        public class Restaurant {
            id;
            owner;
            name;
            description;
            cuisineType;
            address;
            contactInformation;
            openingHours;
            reviews;
            orders;
            numRating;
            images;
            registrationDate;
            open;
            foods;
        }
        ```
        
    - Food
        
        ```jsx
        public class Food {
            id;
            name;
            description;
            price;
            foodCategory;
            images;
            available;
            restaurant;
            isVegetarian;
            isSeasonal;
            ingredients;
            creationDate;
        }
        ```
        
    - Food Category
        
        ```jsx
        public class Category {
            id;
            name;
            restaurant;
        }
        ```
        
    - Ingredients
        
        ```jsx
        public class IngredientCategory {
            id;
            name;
            restaurant;
            ingredients;
        }
        ```
        
        ```jsx
        public class IngredientsItem {
            id;
            name;
            category;
            restaurant;
            inStock;
        }
        ```
        
    - Event
        
        ```jsx
        public class Events {
            id;
            image;
            startedAt;
            endsAt;
            name;
            restaurant;
            location;
        }
        ```
        
    - Order
        
        ```jsx
        public class Order {
            id;
            customer;
            restaurant;
            totalAmount;
            orderStatus;
            createdAt;
            deliveryAddress;
            items;
            payment;
            totalItem;
            totalPrice;
        }
        ```
        
    - order item
        
        ```jsx
        public class OrderItem {
            id;
            food;
            quantity;
            totalPrice;
            ingredients;
        }
        ```
        
    - Cart
        
        ```jsx
        public class Cart {
            id;
            customer;
            items;
            total;
        }
        ```
        
    - Cart Item
        
        ```jsx
        public class CartItem {
            id;
            cart;
            food;
            quantity;
            ingredients;
            totalPrice;
        }
        ```
        
    

# Folder Stucture

project_root/
│
├── src/
│   ├── controllers/        // Controllers handle request/response logic
│   │   ├── itemController.js
│   │   └── ...
│   │
│   ├── models/            // Database models/schema
│   │   ├── itemModel.js
│   │   └── ...
│   │
│   ├── routes/            // API routes
│   │   ├── itemRoutes.js
│   │   └── ...
│   │
│   ├── services/          // Business logic and data processing
│   │   ├── itemService.js
│   │   └── ...
│   │
│   └── app.js             // Entry point of the application
│
├── .env                   // Environment variables
├── package.json           // Project dependencies and metadata
└── ...

- spring boot
    ![Screenshot (265)](https://github.com/user-attachments/assets/2bc6d43d-6547-474c-aec9-b00ca5c1aaa0)
![Screenshot (266)](https://github.com/user-attachments/assets/59662b52-6cd8-4f82-ac7a-bec8876290e2)
![Screenshot (264)](https://github.com/user-attachments/assets/1644cd00-1d46-4174-b36c-0b7cdaa95967)
![Screenshot (262)](https://github.com/user-attachments/assets/1de2aec7-5905-4ace-9a25-ec92dfa0444c)
![Screenshot (261)](https://github.com/user-attachments/assets/276128e5-b0c7-4b64-a9fc-057fccb4ce82)
![Screenshot (260)](https://github.com/user-attachments/assets/f8d09eff-fd88-4a33-b511-0a0169ee0e29)
![Screenshot (258)](https://github.com/user-attachments/assets/61a99f5c-61a5-4510-9301-966c0d9faa69)
![Screenshot (259)](https://github.com/user-attachments/assets/e3396775-a687-4a49-9756-736f57c9e1a7)
![Screenshot (256)](https://github.com/user-attachments/assets/9dd867da-19ef-432b-b62f-6bb9ed7a8e1c)
![Screenshot (255)](https://github.com/user-attachments/assets/81f3d3a8-0d7d-4ad4-83de-78cdb06a2496)
![Screenshot (254)](https://github.com/user-attachments/assets/4eea724a-4a51-4852-93a6-97d9163e173f)


