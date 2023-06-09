API Endpoints
Retrieve All Categories
Retrieves all categories in XML format.

Endpoint: GET /categories
Response Format: XML
Response Body:
<?xml version="1.0" encoding="UTF-8"?>
<document>
    <category>
        <id>1</id>
        <name>LESSONS</name>
        <_lft>1</_lft>
        <_rgt>2</_rgt>
        <parent_id></parent_id>
        <created_at>2023-06-09T09:15:04.000000Z</created_at>
        <updated_at>2023-06-09T09:15:04.000000Z</updated_at>
        <children/>
    </category>
    <category>
        <id>2</id>
        <name>LARAVEL</name>
        <_lft>3</_lft>
        <_rgt>4</_rgt>
        <parent_id></parent_id>
        <created_at>2023-06-09T09:15:04.000000Z</created_at>
        <updated_at>2023-06-09T09:15:04.000000Z</updated_at>
        <children/>
    </category>
</document>

Retrieve a Specific Category
Retrieves a specific category by its ID in XML format.

Endpoint: GET /categories/{id}
Response Format: XML
Response Body:

 <category>
        <id>1</id>
        <name>LESSONS</name>
        <_lft>1</_lft>
        <_rgt>2</_rgt>
        <parent_id></parent_id>
        <created_at>2023-06-09T09:15:04.000000Z</created_at>
        <updated_at>2023-06-09T09:15:04.000000Z</updated_at>
        <children/>
    </category>

Create a New Category
Creates a new category.

Endpoint: POST /categories
Request Format: XML
Request Body:

 <category>
        <id>3</id>
        <name>module</name>
        <_lft>4</_lft>
        <_rgt>5</_rgt>
        <parent_id></parent_id>
        <created_at>2023-06-09T09:15:04.000000Z</created_at>
        <updated_at>2023-06-09T09:15:04.000000Z</updated_at>
        <children/>
    </category>

Update an Existing Category
Updates an existing category by its ID.

Endpoint: PUT /categories/{id}
Request Format: XML
Request Body:


 <category>
        <id>1</id>
        <name>couse</name>
        <_lft>1</_lft>
        <_rgt>2</_rgt>
        <parent_id></parent_id>
        <created_at>2023-06-09T09:15:04.000000Z</created_at>
        <updated_at>2023-06-09T09:15:04.000000Z</updated_at>
        <children/>
    </category>


Delete a Category
Deletes a category by its ID.

Endpoint: DELETE /categories/{id}
Response Format: XML
Response Body:

<message>Category deleted successfully.</message>

Error Handling
The API handles errors and returns appropriate error responses in XML format. For example, if a requested category is not found, the API will respond with:

<error>Category not found.</error>

unit Tests
Unit tests have been implemented to ensure the functionality of the API endpoints. Run the following command to execute the tests:

php artisan test



