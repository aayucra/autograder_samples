def get_address(houses, person):
    for house in houses:
        if hasattr(house, "inhabitants") and person in house.inhabitants:
            return house.address
    return None
