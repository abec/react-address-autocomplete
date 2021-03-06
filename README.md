# react-address-autocomplete (Deprecated)

Deprecated in favor of [react-autosuggest-geocoder](https://github.com/abec/react-autosuggest-geocoder)

Controlled MapZen address autocomplete component for react.

## Example

```
import AddressAutocomplete from 'react-address-autocomplete';

class SearchPage extends React.Component {
  constructor(props) {
    super(props);

    this.state = {
      search: "",
      latitude: Infinity,
      longitude: Infinity
    };
  }

  render() {
    return (
      <div>
        <AddressAutocomplete
          name="location"
          placeholder="Address: 12456 Fake Street #A, San Francisco, CA, 94118"
          value={this.state}
          onChange={data => this.setState(data)}
          apiKey={"..."} />
      </div>
    );
  }
}
```

Check out a demo [here](https://abec.github.io/react-address-autocomplete/)

## Style Guide

Use the following classes as a guide to styling the search input as well as the autocomplete list.

### Search Input

```
.address-autocomplete-container {
  .address-autocomplete-input-container {
    ...
  }
  ...
}
```

### Search Results

```
.collection.autocomplete {
  .collection-item.autocomplete {
    ...
  }
  .collection-item.autocomplete.active {
    ...
  }
  ...
}
```
