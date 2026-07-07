def flatten_list(nested_list):
    flat = []
    for item in nested_list:
        if isinstance(item, list):
            flat.extend(item)
        else:
            flat.append(item)
    return flat

if __name__ == "__main__":
    data = [[1, 2], [3, 4], 5, [6, 7]]
    print(f"Original: {data}")
    print(f"Flattened: {flatten_list(data)}")
