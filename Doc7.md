## Building a better API


We create Address & Profile model
- dto
  
- AddressInput (with class-validator)


```ts
async updateUser(userId: number, firstName: string, lastName: string, userType: string) {
    const queryString = "UPDATE users SET firstName=$1, lastName=$2, userType=$3 WHERE id = userId RETURNING *";
    
    const value = [userId, firstName, lastName, userType];

    const result = await this.executeQuery(queryString, value);

    if(!result) {
        throw new NotFoundException('User not found');
    }

    if(result.rowCount > 0) {
        return result.rows[0] as User;
    }
    
}
```

- ProfileInput